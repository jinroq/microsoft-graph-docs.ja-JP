---
title: settingStateDeviceSummary リソースの種類
description: 設定状態の要約に対する、デバイス コンプライアンス ポリシーおよび構成
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fab849fa44c33996d31ddac15b44c23f8450988d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414838"
---
# <a name="settingstatedevicesummary-resource-type"></a><span data-ttu-id="02c96-103">settingStateDeviceSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="02c96-103">settingStateDeviceSummary resource type</span></span>

> <span data-ttu-id="02c96-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="02c96-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="02c96-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02c96-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="02c96-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="02c96-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02c96-107">設定状態の要約に対する、デバイス コンプライアンス ポリシーおよび構成</span><span class="sxs-lookup"><span data-stu-id="02c96-107">Device Compilance Policy and Configuration for a Setting State summary</span></span>

## <a name="methods"></a><span data-ttu-id="02c96-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="02c96-108">Methods</span></span>
|<span data-ttu-id="02c96-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="02c96-109">Method</span></span>|<span data-ttu-id="02c96-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="02c96-110">Return Type</span></span>|<span data-ttu-id="02c96-111">説明</span><span class="sxs-lookup"><span data-stu-id="02c96-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="02c96-112">settingStateDeviceSummaries のリスト</span><span class="sxs-lookup"><span data-stu-id="02c96-112">List settingStateDeviceSummaries</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|<span data-ttu-id="02c96-113">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="02c96-113">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="02c96-114">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="02c96-114">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>|
|[<span data-ttu-id="02c96-115">settingStateDeviceSummary の取得</span><span class="sxs-lookup"><span data-stu-id="02c96-115">Get settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[<span data-ttu-id="02c96-116">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="02c96-116">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="02c96-117">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="02c96-117">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="02c96-118">settingStateDeviceSummary の作成</span><span class="sxs-lookup"><span data-stu-id="02c96-118">Create settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[<span data-ttu-id="02c96-119">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="02c96-119">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="02c96-120">新しい [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="02c96-120">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="02c96-121">settingStateDeviceSummary の削除</span><span class="sxs-lookup"><span data-stu-id="02c96-121">Delete settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|<span data-ttu-id="02c96-122">なし</span><span class="sxs-lookup"><span data-stu-id="02c96-122">None</span></span>|<span data-ttu-id="02c96-123">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="02c96-123">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>|
|[<span data-ttu-id="02c96-124">settingStateDeviceSummary の更新</span><span class="sxs-lookup"><span data-stu-id="02c96-124">Update settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[<span data-ttu-id="02c96-125">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="02c96-125">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="02c96-126">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="02c96-126">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="02c96-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02c96-127">Properties</span></span>
|<span data-ttu-id="02c96-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02c96-128">Property</span></span>|<span data-ttu-id="02c96-129">型</span><span class="sxs-lookup"><span data-stu-id="02c96-129">Type</span></span>|<span data-ttu-id="02c96-130">説明</span><span class="sxs-lookup"><span data-stu-id="02c96-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02c96-131">id</span><span class="sxs-lookup"><span data-stu-id="02c96-131">id</span></span>|<span data-ttu-id="02c96-132">String</span><span class="sxs-lookup"><span data-stu-id="02c96-132">String</span></span>|<span data-ttu-id="02c96-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="02c96-133">Key of the entity.</span></span>|
|<span data-ttu-id="02c96-134">settingName</span><span class="sxs-lookup"><span data-stu-id="02c96-134">settingName</span></span>|<span data-ttu-id="02c96-135">String</span><span class="sxs-lookup"><span data-stu-id="02c96-135">String</span></span>|<span data-ttu-id="02c96-136">設定の名前</span><span class="sxs-lookup"><span data-stu-id="02c96-136">Name of the setting</span></span>|
|<span data-ttu-id="02c96-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="02c96-137">instancePath</span></span>|<span data-ttu-id="02c96-138">String</span><span class="sxs-lookup"><span data-stu-id="02c96-138">String</span></span>|<span data-ttu-id="02c96-139">設定の InstancePath の名前</span><span class="sxs-lookup"><span data-stu-id="02c96-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="02c96-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02c96-140">unknownDeviceCount</span></span>|<span data-ttu-id="02c96-141">Int32</span><span class="sxs-lookup"><span data-stu-id="02c96-141">Int32</span></span>|<span data-ttu-id="02c96-142">設定の不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="02c96-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="02c96-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02c96-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="02c96-144">Int32</span><span class="sxs-lookup"><span data-stu-id="02c96-144">Int32</span></span>|<span data-ttu-id="02c96-145">設定の該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="02c96-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="02c96-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02c96-146">compliantDeviceCount</span></span>|<span data-ttu-id="02c96-147">Int32</span><span class="sxs-lookup"><span data-stu-id="02c96-147">Int32</span></span>|<span data-ttu-id="02c96-148">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="02c96-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="02c96-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02c96-149">remediatedDeviceCount</span></span>|<span data-ttu-id="02c96-150">Int32</span><span class="sxs-lookup"><span data-stu-id="02c96-150">Int32</span></span>|<span data-ttu-id="02c96-151">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="02c96-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="02c96-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02c96-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="02c96-153">Int32</span><span class="sxs-lookup"><span data-stu-id="02c96-153">Int32</span></span>|<span data-ttu-id="02c96-154">設定の準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="02c96-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="02c96-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02c96-155">errorDeviceCount</span></span>|<span data-ttu-id="02c96-156">Int32</span><span class="sxs-lookup"><span data-stu-id="02c96-156">Int32</span></span>|<span data-ttu-id="02c96-157">設定のデバイス エラーの数</span><span class="sxs-lookup"><span data-stu-id="02c96-157">Device error count for the setting</span></span>|
|<span data-ttu-id="02c96-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02c96-158">conflictDeviceCount</span></span>|<span data-ttu-id="02c96-159">Int32</span><span class="sxs-lookup"><span data-stu-id="02c96-159">Int32</span></span>|<span data-ttu-id="02c96-160">設定のデバイス競合エラーの数</span><span class="sxs-lookup"><span data-stu-id="02c96-160">Device conflict error count for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="02c96-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="02c96-161">Relationships</span></span>
<span data-ttu-id="02c96-162">なし</span><span class="sxs-lookup"><span data-stu-id="02c96-162">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="02c96-163">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="02c96-163">JSON Representation</span></span>
<span data-ttu-id="02c96-164">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="02c96-164">Here is a JSON representation of the resource.</span></span>
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




