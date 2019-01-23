---
title: deviceConfigurationConflictSummary リソースの種類
description: 競合デバイスの構成のポリシーのセットの概要です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7e5f90ddc1b12f052dd603a6979d6838051504aa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418681"
---
# <a name="deviceconfigurationconflictsummary-resource-type"></a><span data-ttu-id="aa462-103">deviceConfigurationConflictSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aa462-103">deviceConfigurationConflictSummary resource type</span></span>

> <span data-ttu-id="aa462-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="aa462-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="aa462-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa462-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aa462-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="aa462-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa462-107">競合デバイスの構成のポリシーのセットの概要です。</span><span class="sxs-lookup"><span data-stu-id="aa462-107">Conflict summary for a set of device configuration policies.</span></span>

## <a name="methods"></a><span data-ttu-id="aa462-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="aa462-108">Methods</span></span>
|<span data-ttu-id="aa462-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="aa462-109">Method</span></span>|<span data-ttu-id="aa462-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="aa462-110">Return Type</span></span>|<span data-ttu-id="aa462-111">説明</span><span class="sxs-lookup"><span data-stu-id="aa462-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aa462-112">リスト deviceConfigurationConflictSummaries</span><span class="sxs-lookup"><span data-stu-id="aa462-112">List deviceConfigurationConflictSummaries</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-list.md)|<span data-ttu-id="aa462-113">[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="aa462-113">[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) collection</span></span>|<span data-ttu-id="aa462-114">[DeviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="aa462-114">List properties and relationships of the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) objects.</span></span>|
|[<span data-ttu-id="aa462-115">DeviceConfigurationConflictSummary を取得します。</span><span class="sxs-lookup"><span data-stu-id="aa462-115">Get deviceConfigurationConflictSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-get.md)|[<span data-ttu-id="aa462-116">deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="aa462-116">deviceConfigurationConflictSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|<span data-ttu-id="aa462-117">[DeviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aa462-117">Read properties and relationships of the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>|
|[<span data-ttu-id="aa462-118">DeviceConfigurationConflictSummary を作成します。</span><span class="sxs-lookup"><span data-stu-id="aa462-118">Create deviceConfigurationConflictSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-create.md)|[<span data-ttu-id="aa462-119">deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="aa462-119">deviceConfigurationConflictSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|<span data-ttu-id="aa462-120">新しい[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="aa462-120">Create a new [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>|
|[<span data-ttu-id="aa462-121">DeviceConfigurationConflictSummary を削除します。</span><span class="sxs-lookup"><span data-stu-id="aa462-121">Delete deviceConfigurationConflictSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-delete.md)|<span data-ttu-id="aa462-122">なし</span><span class="sxs-lookup"><span data-stu-id="aa462-122">None</span></span>|<span data-ttu-id="aa462-123">の[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="aa462-123">Deletes a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>|
|[<span data-ttu-id="aa462-124">DeviceConfigurationConflictSummary を更新します。</span><span class="sxs-lookup"><span data-stu-id="aa462-124">Update deviceConfigurationConflictSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-update.md)|[<span data-ttu-id="aa462-125">deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="aa462-125">deviceConfigurationConflictSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|<span data-ttu-id="aa462-126">[DeviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="aa462-126">Update the properties of a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aa462-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa462-127">Properties</span></span>
|<span data-ttu-id="aa462-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa462-128">Property</span></span>|<span data-ttu-id="aa462-129">型</span><span class="sxs-lookup"><span data-stu-id="aa462-129">Type</span></span>|<span data-ttu-id="aa462-130">説明</span><span class="sxs-lookup"><span data-stu-id="aa462-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa462-131">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="aa462-131">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="aa462-132">[settingSource](../resources/intune-deviceconfig-settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="aa462-132">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="aa462-133">一連のポリシーを指定された設定と競合していません。</span><span class="sxs-lookup"><span data-stu-id="aa462-133">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="aa462-134">id</span><span class="sxs-lookup"><span data-stu-id="aa462-134">id</span></span>|<span data-ttu-id="aa462-135">String</span><span class="sxs-lookup"><span data-stu-id="aa462-135">String</span></span>|<span data-ttu-id="aa462-136">競合するポリシーのセットの id です。</span><span class="sxs-lookup"><span data-stu-id="aa462-136">The id for this set of conflicting policies.</span></span> <span data-ttu-id="aa462-137">この id では、ConflictingDeviceConfigurations 内のすべてのポリシーの id をアンダー スコアで区切られた辞書式の順序にします。</span><span class="sxs-lookup"><span data-stu-id="aa462-137">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="aa462-138">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="aa462-138">contributingSettings</span></span>|<span data-ttu-id="aa462-139">String コレクション</span><span class="sxs-lookup"><span data-stu-id="aa462-139">String collection</span></span>|<span data-ttu-id="aa462-140">一連の特定のポリシーと競合の設定</span><span class="sxs-lookup"><span data-stu-id="aa462-140">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="aa462-141">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="aa462-141">deviceCheckinsImpacted</span></span>|<span data-ttu-id="aa462-142">Int32</span><span class="sxs-lookup"><span data-stu-id="aa462-142">Int32</span></span>|<span data-ttu-id="aa462-143">チェックインの競合しているポリシーと設定の影響を受ける数</span><span class="sxs-lookup"><span data-stu-id="aa462-143">The count of checkins impacted by the conflicting policies and settings</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa462-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aa462-144">Relationships</span></span>
<span data-ttu-id="aa462-145">なし</span><span class="sxs-lookup"><span data-stu-id="aa462-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa462-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aa462-146">JSON Representation</span></span>
<span data-ttu-id="aa462-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aa462-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationConflictSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "String",
      "displayName": "String"
    }
  ],
  "id": "String (identifier)",
  "contributingSettings": [
    "String"
  ],
  "deviceCheckinsImpacted": 1024
}
```




