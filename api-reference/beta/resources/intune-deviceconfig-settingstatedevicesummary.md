---
title: settingStateDeviceSummary リソースの種類
description: 設定状態の要約に対する、デバイス コンプライアンス ポリシーおよび構成
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 26d0c2d39d79a81e419141087e508497c91f4e03
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944734"
---
# <a name="settingstatedevicesummary-resource-type"></a><span data-ttu-id="60e29-103">settingStateDeviceSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="60e29-103">settingStateDeviceSummary resource type</span></span>

> <span data-ttu-id="60e29-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60e29-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60e29-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="60e29-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60e29-106">設定状態の要約に対する、デバイス コンプライアンス ポリシーおよび構成</span><span class="sxs-lookup"><span data-stu-id="60e29-106">Device Compilance Policy and Configuration for a Setting State summary</span></span>

## <a name="methods"></a><span data-ttu-id="60e29-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="60e29-107">Methods</span></span>
|<span data-ttu-id="60e29-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="60e29-108">Method</span></span>|<span data-ttu-id="60e29-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="60e29-109">Return Type</span></span>|<span data-ttu-id="60e29-110">説明</span><span class="sxs-lookup"><span data-stu-id="60e29-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="60e29-111">settingStateDeviceSummaries のリスト</span><span class="sxs-lookup"><span data-stu-id="60e29-111">List settingStateDeviceSummaries</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|<span data-ttu-id="60e29-112">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="60e29-112">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="60e29-113">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="60e29-113">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>|
|[<span data-ttu-id="60e29-114">settingStateDeviceSummary の取得</span><span class="sxs-lookup"><span data-stu-id="60e29-114">Get settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[<span data-ttu-id="60e29-115">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="60e29-115">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="60e29-116">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="60e29-116">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="60e29-117">settingStateDeviceSummary の作成</span><span class="sxs-lookup"><span data-stu-id="60e29-117">Create settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[<span data-ttu-id="60e29-118">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="60e29-118">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="60e29-119">新しい [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="60e29-119">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="60e29-120">settingStateDeviceSummary の削除</span><span class="sxs-lookup"><span data-stu-id="60e29-120">Delete settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|<span data-ttu-id="60e29-121">なし</span><span class="sxs-lookup"><span data-stu-id="60e29-121">None</span></span>|<span data-ttu-id="60e29-122">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="60e29-122">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>|
|[<span data-ttu-id="60e29-123">settingStateDeviceSummary の更新</span><span class="sxs-lookup"><span data-stu-id="60e29-123">Update settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[<span data-ttu-id="60e29-124">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="60e29-124">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="60e29-125">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="60e29-125">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="60e29-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60e29-126">Properties</span></span>
|<span data-ttu-id="60e29-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60e29-127">Property</span></span>|<span data-ttu-id="60e29-128">型</span><span class="sxs-lookup"><span data-stu-id="60e29-128">Type</span></span>|<span data-ttu-id="60e29-129">説明</span><span class="sxs-lookup"><span data-stu-id="60e29-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60e29-130">id</span><span class="sxs-lookup"><span data-stu-id="60e29-130">id</span></span>|<span data-ttu-id="60e29-131">String</span><span class="sxs-lookup"><span data-stu-id="60e29-131">String</span></span>|<span data-ttu-id="60e29-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="60e29-132">Key of the entity.</span></span>|
|<span data-ttu-id="60e29-133">settingName</span><span class="sxs-lookup"><span data-stu-id="60e29-133">settingName</span></span>|<span data-ttu-id="60e29-134">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="60e29-134">String</span></span>|<span data-ttu-id="60e29-135">設定の名前</span><span class="sxs-lookup"><span data-stu-id="60e29-135">Name of the setting</span></span>|
|<span data-ttu-id="60e29-136">instancePath</span><span class="sxs-lookup"><span data-stu-id="60e29-136">instancePath</span></span>|<span data-ttu-id="60e29-137">String</span><span class="sxs-lookup"><span data-stu-id="60e29-137">String</span></span>|<span data-ttu-id="60e29-138">設定の InstancePath の名前</span><span class="sxs-lookup"><span data-stu-id="60e29-138">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="60e29-139">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="60e29-139">unknownDeviceCount</span></span>|<span data-ttu-id="60e29-140">Int32</span><span class="sxs-lookup"><span data-stu-id="60e29-140">Int32</span></span>|<span data-ttu-id="60e29-141">設定の不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="60e29-141">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="60e29-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="60e29-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="60e29-143">Int32</span><span class="sxs-lookup"><span data-stu-id="60e29-143">Int32</span></span>|<span data-ttu-id="60e29-144">設定の該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="60e29-144">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="60e29-145">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="60e29-145">compliantDeviceCount</span></span>|<span data-ttu-id="60e29-146">Int32</span><span class="sxs-lookup"><span data-stu-id="60e29-146">Int32</span></span>|<span data-ttu-id="60e29-147">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="60e29-147">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="60e29-148">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="60e29-148">remediatedDeviceCount</span></span>|<span data-ttu-id="60e29-149">Int32</span><span class="sxs-lookup"><span data-stu-id="60e29-149">Int32</span></span>|<span data-ttu-id="60e29-150">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="60e29-150">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="60e29-151">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="60e29-151">nonCompliantDeviceCount</span></span>|<span data-ttu-id="60e29-152">Int32</span><span class="sxs-lookup"><span data-stu-id="60e29-152">Int32</span></span>|<span data-ttu-id="60e29-153">設定の準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="60e29-153">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="60e29-154">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="60e29-154">errorDeviceCount</span></span>|<span data-ttu-id="60e29-155">Int32</span><span class="sxs-lookup"><span data-stu-id="60e29-155">Int32</span></span>|<span data-ttu-id="60e29-156">設定のデバイス エラーの数</span><span class="sxs-lookup"><span data-stu-id="60e29-156">Device error count for the setting</span></span>|
|<span data-ttu-id="60e29-157">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="60e29-157">conflictDeviceCount</span></span>|<span data-ttu-id="60e29-158">Int32</span><span class="sxs-lookup"><span data-stu-id="60e29-158">Int32</span></span>|<span data-ttu-id="60e29-159">設定のデバイス競合エラーの数</span><span class="sxs-lookup"><span data-stu-id="60e29-159">Device conflict error count for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="60e29-160">関係</span><span class="sxs-lookup"><span data-stu-id="60e29-160">Relationships</span></span>
<span data-ttu-id="60e29-161">なし</span><span class="sxs-lookup"><span data-stu-id="60e29-161">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="60e29-162">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="60e29-162">JSON Representation</span></span>
<span data-ttu-id="60e29-163">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="60e29-163">Here is a JSON representation of the resource.</span></span>
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




