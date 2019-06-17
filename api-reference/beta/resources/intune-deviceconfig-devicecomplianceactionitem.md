---
title: deviceComplianceActionItem リソース タイプ
description: スケジュール済みのアクションの構成
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e27d2fb5e8822dc4adc8503bbc6731e573c87759
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979537"
---
# <a name="devicecomplianceactionitem-resource-type"></a><span data-ttu-id="c8dc6-103">deviceComplianceActionItem リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="c8dc6-103">deviceComplianceActionItem resource type</span></span>

> <span data-ttu-id="c8dc6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8dc6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8dc6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c8dc6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8dc6-106">スケジュール済みのアクションの構成</span><span class="sxs-lookup"><span data-stu-id="c8dc6-106">Scheduled Action Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="c8dc6-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c8dc6-107">Methods</span></span>
|<span data-ttu-id="c8dc6-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c8dc6-108">Method</span></span>|<span data-ttu-id="c8dc6-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c8dc6-109">Return Type</span></span>|<span data-ttu-id="c8dc6-110">説明</span><span class="sxs-lookup"><span data-stu-id="c8dc6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c8dc6-111">List deviceComplianceActionItems</span><span class="sxs-lookup"><span data-stu-id="c8dc6-111">List deviceComplianceActionItems</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-list.md)|<span data-ttu-id="c8dc6-112">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c8dc6-112">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) collection</span></span>|<span data-ttu-id="c8dc6-113">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c8dc6-113">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>|
|[<span data-ttu-id="c8dc6-114">Get deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="c8dc6-114">Get deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-get.md)|[<span data-ttu-id="c8dc6-115">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="c8dc6-115">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="c8dc6-116">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c8dc6-116">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="c8dc6-117">Create deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="c8dc6-117">Create deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-create.md)|[<span data-ttu-id="c8dc6-118">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="c8dc6-118">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="c8dc6-119">新しい [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c8dc6-119">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="c8dc6-120">Delete deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="c8dc6-120">Delete deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-delete.md)|<span data-ttu-id="c8dc6-121">なし</span><span class="sxs-lookup"><span data-stu-id="c8dc6-121">None</span></span>|<span data-ttu-id="c8dc6-122">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="c8dc6-122">Deletes a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>|
|[<span data-ttu-id="c8dc6-123">Update deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="c8dc6-123">Update deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-update.md)|[<span data-ttu-id="c8dc6-124">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="c8dc6-124">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="c8dc6-125">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c8dc6-125">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c8dc6-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8dc6-126">Properties</span></span>
|<span data-ttu-id="c8dc6-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8dc6-127">Property</span></span>|<span data-ttu-id="c8dc6-128">型</span><span class="sxs-lookup"><span data-stu-id="c8dc6-128">Type</span></span>|<span data-ttu-id="c8dc6-129">説明</span><span class="sxs-lookup"><span data-stu-id="c8dc6-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8dc6-130">id</span><span class="sxs-lookup"><span data-stu-id="c8dc6-130">id</span></span>|<span data-ttu-id="c8dc6-131">String</span><span class="sxs-lookup"><span data-stu-id="c8dc6-131">String</span></span>|<span data-ttu-id="c8dc6-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c8dc6-132">Key of the entity.</span></span>|
|<span data-ttu-id="c8dc6-133">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="c8dc6-133">gracePeriodHours</span></span>|<span data-ttu-id="c8dc6-134">Int32</span><span class="sxs-lookup"><span data-stu-id="c8dc6-134">Int32</span></span>|<span data-ttu-id="c8dc6-135">アクションが実行されるまでの待機時間。</span><span class="sxs-lookup"><span data-stu-id="c8dc6-135">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="c8dc6-136">有効な値は 0 から 8760 までです</span><span class="sxs-lookup"><span data-stu-id="c8dc6-136">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="c8dc6-137">actionType</span><span class="sxs-lookup"><span data-stu-id="c8dc6-137">actionType</span></span>|[<span data-ttu-id="c8dc6-138">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="c8dc6-138">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="c8dc6-139">実行するアクション。</span><span class="sxs-lookup"><span data-stu-id="c8dc6-139">What action to take.</span></span> <span data-ttu-id="c8dc6-140">可能な値は、`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock` です。</span><span class="sxs-lookup"><span data-stu-id="c8dc6-140">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="c8dc6-141">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="c8dc6-141">notificationTemplateId</span></span>|<span data-ttu-id="c8dc6-142">String</span><span class="sxs-lookup"><span data-stu-id="c8dc6-142">String</span></span>|<span data-ttu-id="c8dc6-143">使用する通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="c8dc6-143">What notification Message template to use</span></span>|
|<span data-ttu-id="c8dc6-144">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="c8dc6-144">notificationMessageCCList</span></span>|<span data-ttu-id="c8dc6-145">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c8dc6-145">String collection</span></span>|<span data-ttu-id="c8dc6-146">この通知メッセージの CC に設定するグループ ID のリスト。</span><span class="sxs-lookup"><span data-stu-id="c8dc6-146">A list of group IDs to speicify who to CC this notification message to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8dc6-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c8dc6-147">Relationships</span></span>
<span data-ttu-id="c8dc6-148">なし</span><span class="sxs-lookup"><span data-stu-id="c8dc6-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8dc6-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c8dc6-149">JSON Representation</span></span>
<span data-ttu-id="c8dc6-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c8dc6-150">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceActionItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "id": "String (identifier)",
  "gracePeriodHours": 1024,
  "actionType": "String",
  "notificationTemplateId": "String",
  "notificationMessageCCList": [
    "String"
  ]
}
```





