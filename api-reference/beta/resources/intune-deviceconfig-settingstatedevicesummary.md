---
title: settingStateDeviceSummary リソースの種類
description: 設定状態の要約に対する、デバイス コンプライアンス ポリシーおよび構成
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f233b285fa9967dca03406c3ca7c649773e9832
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782682"
---
# <a name="settingstatedevicesummary-resource-type"></a><span data-ttu-id="6a977-103">settingStateDeviceSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6a977-103">settingStateDeviceSummary resource type</span></span>

> <span data-ttu-id="6a977-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a977-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a977-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6a977-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a977-106">設定状態の要約に対する、デバイス コンプライアンス ポリシーおよび構成</span><span class="sxs-lookup"><span data-stu-id="6a977-106">Device Compilance Policy and Configuration for a Setting State summary</span></span>

## <a name="methods"></a><span data-ttu-id="6a977-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="6a977-107">Methods</span></span>
|<span data-ttu-id="6a977-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="6a977-108">Method</span></span>|<span data-ttu-id="6a977-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6a977-109">Return Type</span></span>|<span data-ttu-id="6a977-110">説明</span><span class="sxs-lookup"><span data-stu-id="6a977-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6a977-111">settingStateDeviceSummaries のリスト</span><span class="sxs-lookup"><span data-stu-id="6a977-111">List settingStateDeviceSummaries</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|<span data-ttu-id="6a977-112">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6a977-112">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="6a977-113">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6a977-113">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>|
|[<span data-ttu-id="6a977-114">Get settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6a977-114">Get settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[<span data-ttu-id="6a977-115">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6a977-115">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="6a977-116">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6a977-116">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="6a977-117">settingStateDeviceSummary の作成</span><span class="sxs-lookup"><span data-stu-id="6a977-117">Create settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[<span data-ttu-id="6a977-118">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6a977-118">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="6a977-119">新しい [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6a977-119">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="6a977-120">settingStateDeviceSummary の削除</span><span class="sxs-lookup"><span data-stu-id="6a977-120">Delete settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|<span data-ttu-id="6a977-121">なし</span><span class="sxs-lookup"><span data-stu-id="6a977-121">None</span></span>|<span data-ttu-id="6a977-122">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="6a977-122">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>|
|[<span data-ttu-id="6a977-123">settingStateDeviceSummary の更新</span><span class="sxs-lookup"><span data-stu-id="6a977-123">Update settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[<span data-ttu-id="6a977-124">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6a977-124">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="6a977-125">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6a977-125">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6a977-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a977-126">Properties</span></span>
|<span data-ttu-id="6a977-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a977-127">Property</span></span>|<span data-ttu-id="6a977-128">型</span><span class="sxs-lookup"><span data-stu-id="6a977-128">Type</span></span>|<span data-ttu-id="6a977-129">説明</span><span class="sxs-lookup"><span data-stu-id="6a977-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a977-130">id</span><span class="sxs-lookup"><span data-stu-id="6a977-130">id</span></span>|<span data-ttu-id="6a977-131">String</span><span class="sxs-lookup"><span data-stu-id="6a977-131">String</span></span>|<span data-ttu-id="6a977-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6a977-132">Key of the entity.</span></span>|
|<span data-ttu-id="6a977-133">settingName</span><span class="sxs-lookup"><span data-stu-id="6a977-133">settingName</span></span>|<span data-ttu-id="6a977-134">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="6a977-134">String</span></span>|<span data-ttu-id="6a977-135">設定の名前</span><span class="sxs-lookup"><span data-stu-id="6a977-135">Name of the setting</span></span>|
|<span data-ttu-id="6a977-136">instancePath</span><span class="sxs-lookup"><span data-stu-id="6a977-136">instancePath</span></span>|<span data-ttu-id="6a977-137">String</span><span class="sxs-lookup"><span data-stu-id="6a977-137">String</span></span>|<span data-ttu-id="6a977-138">設定の InstancePath の名前</span><span class="sxs-lookup"><span data-stu-id="6a977-138">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="6a977-139">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6a977-139">unknownDeviceCount</span></span>|<span data-ttu-id="6a977-140">Int32</span><span class="sxs-lookup"><span data-stu-id="6a977-140">Int32</span></span>|<span data-ttu-id="6a977-141">設定の不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="6a977-141">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="6a977-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6a977-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="6a977-143">Int32</span><span class="sxs-lookup"><span data-stu-id="6a977-143">Int32</span></span>|<span data-ttu-id="6a977-144">設定の該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="6a977-144">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="6a977-145">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6a977-145">compliantDeviceCount</span></span>|<span data-ttu-id="6a977-146">Int32</span><span class="sxs-lookup"><span data-stu-id="6a977-146">Int32</span></span>|<span data-ttu-id="6a977-147">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="6a977-147">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="6a977-148">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6a977-148">remediatedDeviceCount</span></span>|<span data-ttu-id="6a977-149">Int32</span><span class="sxs-lookup"><span data-stu-id="6a977-149">Int32</span></span>|<span data-ttu-id="6a977-150">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="6a977-150">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="6a977-151">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6a977-151">nonCompliantDeviceCount</span></span>|<span data-ttu-id="6a977-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6a977-152">Int32</span></span>|<span data-ttu-id="6a977-153">設定の準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="6a977-153">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="6a977-154">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6a977-154">errorDeviceCount</span></span>|<span data-ttu-id="6a977-155">Int32</span><span class="sxs-lookup"><span data-stu-id="6a977-155">Int32</span></span>|<span data-ttu-id="6a977-156">設定のデバイス エラーの数</span><span class="sxs-lookup"><span data-stu-id="6a977-156">Device error count for the setting</span></span>|
|<span data-ttu-id="6a977-157">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6a977-157">conflictDeviceCount</span></span>|<span data-ttu-id="6a977-158">Int32</span><span class="sxs-lookup"><span data-stu-id="6a977-158">Int32</span></span>|<span data-ttu-id="6a977-159">設定のデバイス競合エラーの数</span><span class="sxs-lookup"><span data-stu-id="6a977-159">Device conflict error count for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a977-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6a977-160">Relationships</span></span>
<span data-ttu-id="6a977-161">なし</span><span class="sxs-lookup"><span data-stu-id="6a977-161">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a977-162">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6a977-162">JSON Representation</span></span>
<span data-ttu-id="6a977-163">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6a977-163">Here is a JSON representation of the resource.</span></span>
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





