---
title: deviceConfigurationConflictSummary リソースの種類
description: 競合デバイスの構成のポリシーのセットの概要です。
author: tfitzmac
ms.openlocfilehash: 1c0caefc497c18fe7a8504324e048cec0e53bd3c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308989"
---
# <a name="deviceconfigurationconflictsummary-resource-type"></a><span data-ttu-id="6c3a9-103">deviceConfigurationConflictSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6c3a9-103">deviceConfigurationConflictSummary resource type</span></span>

> <span data-ttu-id="6c3a9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6c3a9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c3a9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c3a9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6c3a9-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6c3a9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c3a9-107">競合デバイスの構成のポリシーのセットの概要です。</span><span class="sxs-lookup"><span data-stu-id="6c3a9-107">Conflict summary for a set of device configuration policies.</span></span>
## <a name="methods"></a><span data-ttu-id="6c3a9-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="6c3a9-108">Methods</span></span>
|<span data-ttu-id="6c3a9-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="6c3a9-109">Method</span></span>|<span data-ttu-id="6c3a9-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6c3a9-110">Return Type</span></span>|<span data-ttu-id="6c3a9-111">説明</span><span class="sxs-lookup"><span data-stu-id="6c3a9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6c3a9-112">リスト deviceConfigurationConflictSummaries</span><span class="sxs-lookup"><span data-stu-id="6c3a9-112">List deviceConfigurationConflictSummaries</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-list.md)|<span data-ttu-id="6c3a9-113">[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6c3a9-113">[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) collection</span></span>|<span data-ttu-id="6c3a9-114">[DeviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="6c3a9-114">List properties and relationships of the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) objects.</span></span>|
|[<span data-ttu-id="6c3a9-115">DeviceConfigurationConflictSummary を取得します。</span><span class="sxs-lookup"><span data-stu-id="6c3a9-115">Get deviceConfigurationConflictSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-get.md)|[<span data-ttu-id="6c3a9-116">deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="6c3a9-116">deviceConfigurationConflictSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|<span data-ttu-id="6c3a9-117">[DeviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c3a9-117">Read properties and relationships of the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>|
|[<span data-ttu-id="6c3a9-118">DeviceConfigurationConflictSummary を作成します。</span><span class="sxs-lookup"><span data-stu-id="6c3a9-118">Create deviceConfigurationConflictSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-create.md)|[<span data-ttu-id="6c3a9-119">deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="6c3a9-119">deviceConfigurationConflictSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|<span data-ttu-id="6c3a9-120">新しい[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6c3a9-120">Create a new [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>|
|[<span data-ttu-id="6c3a9-121">DeviceConfigurationConflictSummary を削除します。</span><span class="sxs-lookup"><span data-stu-id="6c3a9-121">Delete deviceConfigurationConflictSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-delete.md)|<span data-ttu-id="6c3a9-122">なし</span><span class="sxs-lookup"><span data-stu-id="6c3a9-122">None</span></span>|<span data-ttu-id="6c3a9-123">の[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="6c3a9-123">Deletes a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>|
|[<span data-ttu-id="6c3a9-124">DeviceConfigurationConflictSummary を更新します。</span><span class="sxs-lookup"><span data-stu-id="6c3a9-124">Update deviceConfigurationConflictSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-update.md)|[<span data-ttu-id="6c3a9-125">deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="6c3a9-125">deviceConfigurationConflictSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|<span data-ttu-id="6c3a9-126">[DeviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6c3a9-126">Update the properties of a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6c3a9-127">Properties</span><span class="sxs-lookup"><span data-stu-id="6c3a9-127">Properties</span></span>
|<span data-ttu-id="6c3a9-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c3a9-128">Property</span></span>|<span data-ttu-id="6c3a9-129">種類</span><span class="sxs-lookup"><span data-stu-id="6c3a9-129">Type</span></span>|<span data-ttu-id="6c3a9-130">説明</span><span class="sxs-lookup"><span data-stu-id="6c3a9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c3a9-131">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="6c3a9-131">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="6c3a9-132">[settingSource](../resources/intune-deviceconfig-settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6c3a9-132">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="6c3a9-133">一連のポリシーを指定された設定と競合していません。</span><span class="sxs-lookup"><span data-stu-id="6c3a9-133">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="6c3a9-134">id</span><span class="sxs-lookup"><span data-stu-id="6c3a9-134">id</span></span>|<span data-ttu-id="6c3a9-135">String</span><span class="sxs-lookup"><span data-stu-id="6c3a9-135">String</span></span>|<span data-ttu-id="6c3a9-136">競合するポリシーのセットの id です。</span><span class="sxs-lookup"><span data-stu-id="6c3a9-136">The id for this set of conflicting policies.</span></span> <span data-ttu-id="6c3a9-137">この id では、ConflictingDeviceConfigurations 内のすべてのポリシーの id をアンダー スコアで区切られた辞書式の順序にします。</span><span class="sxs-lookup"><span data-stu-id="6c3a9-137">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="6c3a9-138">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="6c3a9-138">contributingSettings</span></span>|<span data-ttu-id="6c3a9-139">String コレクション</span><span class="sxs-lookup"><span data-stu-id="6c3a9-139">String collection</span></span>|<span data-ttu-id="6c3a9-140">一連の特定のポリシーと競合の設定</span><span class="sxs-lookup"><span data-stu-id="6c3a9-140">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="6c3a9-141">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="6c3a9-141">deviceCheckinsImpacted</span></span>|<span data-ttu-id="6c3a9-142">Int32</span><span class="sxs-lookup"><span data-stu-id="6c3a9-142">Int32</span></span>|<span data-ttu-id="6c3a9-143">チェックインの競合しているポリシーと設定の影響を受ける数</span><span class="sxs-lookup"><span data-stu-id="6c3a9-143">The count of checkins impacted by the conflicting policies and settings</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c3a9-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6c3a9-144">Relationships</span></span>
<span data-ttu-id="6c3a9-145">なし</span><span class="sxs-lookup"><span data-stu-id="6c3a9-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6c3a9-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6c3a9-146">JSON Representation</span></span>
<span data-ttu-id="6c3a9-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6c3a9-147">Here is a JSON representation of the resource.</span></span>
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





