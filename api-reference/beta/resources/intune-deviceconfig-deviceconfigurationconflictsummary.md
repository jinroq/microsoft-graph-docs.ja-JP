---
title: deviceConfigurationConflictSummary リソースの種類
description: 一連のデバイス構成ポリシーの競合の概要。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3ce50b49c34427f1cde7011fb76e566a1e45ba9f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333017"
---
# <a name="deviceconfigurationconflictsummary-resource-type"></a><span data-ttu-id="1e55e-103">deviceConfigurationConflictSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1e55e-103">deviceConfigurationConflictSummary resource type</span></span>

> <span data-ttu-id="1e55e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e55e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e55e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1e55e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e55e-106">一連のデバイス構成ポリシーの競合の概要。</span><span class="sxs-lookup"><span data-stu-id="1e55e-106">Conflict summary for a set of device configuration policies.</span></span>

## <a name="methods"></a><span data-ttu-id="1e55e-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="1e55e-107">Methods</span></span>
|<span data-ttu-id="1e55e-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="1e55e-108">Method</span></span>|<span data-ttu-id="1e55e-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1e55e-109">Return Type</span></span>|<span data-ttu-id="1e55e-110">説明</span><span class="sxs-lookup"><span data-stu-id="1e55e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1e55e-111">リスト deviceConfigurationConflictSummaries</span><span class="sxs-lookup"><span data-stu-id="1e55e-111">List deviceConfigurationConflictSummaries</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-list.md)|<span data-ttu-id="1e55e-112">[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1e55e-112">[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) collection</span></span>|<span data-ttu-id="1e55e-113">[DeviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="1e55e-113">List properties and relationships of the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) objects.</span></span>|
|[<span data-ttu-id="1e55e-114">DeviceConfigurationConflictSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="1e55e-114">Get deviceConfigurationConflictSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-get.md)|[<span data-ttu-id="1e55e-115">deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="1e55e-115">deviceConfigurationConflictSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|<span data-ttu-id="1e55e-116">[DeviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1e55e-116">Read properties and relationships of the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>|
|[<span data-ttu-id="1e55e-117">DeviceConfigurationConflictSummary を作成する</span><span class="sxs-lookup"><span data-stu-id="1e55e-117">Create deviceConfigurationConflictSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-create.md)|[<span data-ttu-id="1e55e-118">deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="1e55e-118">deviceConfigurationConflictSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|<span data-ttu-id="1e55e-119">新しい[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1e55e-119">Create a new [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>|
|[<span data-ttu-id="1e55e-120">DeviceConfigurationConflictSummary の削除</span><span class="sxs-lookup"><span data-stu-id="1e55e-120">Delete deviceConfigurationConflictSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-delete.md)|<span data-ttu-id="1e55e-121">None</span><span class="sxs-lookup"><span data-stu-id="1e55e-121">None</span></span>|<span data-ttu-id="1e55e-122">[DeviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="1e55e-122">Deletes a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>|
|[<span data-ttu-id="1e55e-123">DeviceConfigurationConflictSummary の更新</span><span class="sxs-lookup"><span data-stu-id="1e55e-123">Update deviceConfigurationConflictSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-update.md)|[<span data-ttu-id="1e55e-124">deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="1e55e-124">deviceConfigurationConflictSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|<span data-ttu-id="1e55e-125">[DeviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1e55e-125">Update the properties of a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1e55e-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e55e-126">Properties</span></span>
|<span data-ttu-id="1e55e-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e55e-127">Property</span></span>|<span data-ttu-id="1e55e-128">型</span><span class="sxs-lookup"><span data-stu-id="1e55e-128">Type</span></span>|<span data-ttu-id="1e55e-129">説明</span><span class="sxs-lookup"><span data-stu-id="1e55e-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e55e-130">競合する Devicdeviceconfigurん</span><span class="sxs-lookup"><span data-stu-id="1e55e-130">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="1e55e-131">[settingSource](../resources/intune-deviceconfig-settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1e55e-131">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="1e55e-132">指定された設定と競合しているポリシーのセット</span><span class="sxs-lookup"><span data-stu-id="1e55e-132">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="1e55e-133">id</span><span class="sxs-lookup"><span data-stu-id="1e55e-133">id</span></span>|<span data-ttu-id="1e55e-134">String</span><span class="sxs-lookup"><span data-stu-id="1e55e-134">String</span></span>|<span data-ttu-id="1e55e-135">競合しているポリシーのセットの id。</span><span class="sxs-lookup"><span data-stu-id="1e55e-135">The id for this set of conflicting policies.</span></span> <span data-ttu-id="1e55e-136">この id は、アンダースコアで区切られた辞書順で競合しているすべてのポリシーの id です。</span><span class="sxs-lookup"><span data-stu-id="1e55e-136">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="1e55e-137">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="1e55e-137">contributingSettings</span></span>|<span data-ttu-id="1e55e-138">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="1e55e-138">String collection</span></span>|<span data-ttu-id="1e55e-139">指定されたポリシーと競合する設定のセット</span><span class="sxs-lookup"><span data-stu-id="1e55e-139">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="1e55e-140">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="1e55e-140">deviceCheckinsImpacted</span></span>|<span data-ttu-id="1e55e-141">Int32</span><span class="sxs-lookup"><span data-stu-id="1e55e-141">Int32</span></span>|<span data-ttu-id="1e55e-142">競合するポリシーと設定によって影響を受けるチェックインの数</span><span class="sxs-lookup"><span data-stu-id="1e55e-142">The count of checkins impacted by the conflicting policies and settings</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e55e-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1e55e-143">Relationships</span></span>
<span data-ttu-id="1e55e-144">なし</span><span class="sxs-lookup"><span data-stu-id="1e55e-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e55e-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1e55e-145">JSON Representation</span></span>
<span data-ttu-id="1e55e-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1e55e-146">Here is a JSON representation of the resource.</span></span>
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



