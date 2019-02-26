---
title: deviceComplianceActionItem リソース タイプ
description: スケジュール済みのアクションの構成
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1b0a507ffb080f2354e5c854810554da64b47e7c
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254689"
---
# <a name="devicecomplianceactionitem-resource-type"></a><span data-ttu-id="cbed4-103">deviceComplianceActionItem リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="cbed4-103">deviceComplianceActionItem resource type</span></span>

> <span data-ttu-id="cbed4-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cbed4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbed4-105">スケジュール済みのアクションの構成</span><span class="sxs-lookup"><span data-stu-id="cbed4-105">Scheduled Action Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="cbed4-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="cbed4-106">Methods</span></span>
|<span data-ttu-id="cbed4-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="cbed4-107">Method</span></span>|<span data-ttu-id="cbed4-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cbed4-108">Return Type</span></span>|<span data-ttu-id="cbed4-109">説明</span><span class="sxs-lookup"><span data-stu-id="cbed4-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cbed4-110">List deviceComplianceActionItems</span><span class="sxs-lookup"><span data-stu-id="cbed4-110">List deviceComplianceActionItems</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-list.md)|<span data-ttu-id="cbed4-111">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cbed4-111">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) collection</span></span>|<span data-ttu-id="cbed4-112">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="cbed4-112">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>|
|[<span data-ttu-id="cbed4-113">Get deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="cbed4-113">Get deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-get.md)|[<span data-ttu-id="cbed4-114">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="cbed4-114">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="cbed4-115">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="cbed4-115">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="cbed4-116">Create deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="cbed4-116">Create deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-create.md)|[<span data-ttu-id="cbed4-117">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="cbed4-117">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="cbed4-118">新しい [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cbed4-118">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="cbed4-119">Delete deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="cbed4-119">Delete deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-delete.md)|<span data-ttu-id="cbed4-120">なし</span><span class="sxs-lookup"><span data-stu-id="cbed4-120">None</span></span>|<span data-ttu-id="cbed4-121">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="cbed4-121">Deletes a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>|
|[<span data-ttu-id="cbed4-122">Update deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="cbed4-122">Update deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-update.md)|[<span data-ttu-id="cbed4-123">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="cbed4-123">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="cbed4-124">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cbed4-124">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cbed4-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cbed4-125">Properties</span></span>
|<span data-ttu-id="cbed4-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cbed4-126">Property</span></span>|<span data-ttu-id="cbed4-127">型</span><span class="sxs-lookup"><span data-stu-id="cbed4-127">Type</span></span>|<span data-ttu-id="cbed4-128">説明</span><span class="sxs-lookup"><span data-stu-id="cbed4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbed4-129">id</span><span class="sxs-lookup"><span data-stu-id="cbed4-129">id</span></span>|<span data-ttu-id="cbed4-130">String</span><span class="sxs-lookup"><span data-stu-id="cbed4-130">String</span></span>|<span data-ttu-id="cbed4-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cbed4-131">Key of the entity.</span></span>|
|<span data-ttu-id="cbed4-132">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="cbed4-132">gracePeriodHours</span></span>|<span data-ttu-id="cbed4-133">Int32</span><span class="sxs-lookup"><span data-stu-id="cbed4-133">Int32</span></span>|<span data-ttu-id="cbed4-134">アクションが実行されるまでの待機時間。</span><span class="sxs-lookup"><span data-stu-id="cbed4-134">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="cbed4-135">有効な値は 0 から 8760 までです</span><span class="sxs-lookup"><span data-stu-id="cbed4-135">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="cbed4-136">actionType</span><span class="sxs-lookup"><span data-stu-id="cbed4-136">actionType</span></span>|[<span data-ttu-id="cbed4-137">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="cbed4-137">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="cbed4-138">実行するアクション。</span><span class="sxs-lookup"><span data-stu-id="cbed4-138">What action to take.</span></span> <span data-ttu-id="cbed4-139">可能な値は、`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification` です。</span><span class="sxs-lookup"><span data-stu-id="cbed4-139">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="cbed4-140">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="cbed4-140">notificationTemplateId</span></span>|<span data-ttu-id="cbed4-141">String</span><span class="sxs-lookup"><span data-stu-id="cbed4-141">String</span></span>|<span data-ttu-id="cbed4-142">使用する通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="cbed4-142">What notification Message template to use</span></span>|
|<span data-ttu-id="cbed4-143">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="cbed4-143">notificationMessageCCList</span></span>|<span data-ttu-id="cbed4-144">String コレクション</span><span class="sxs-lookup"><span data-stu-id="cbed4-144">String collection</span></span>|<span data-ttu-id="cbed4-145">この通知メッセージの CC に設定するグループ ID のリスト。</span><span class="sxs-lookup"><span data-stu-id="cbed4-145">A list of group IDs to speicify who to CC this notification message to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cbed4-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cbed4-146">Relationships</span></span>
<span data-ttu-id="cbed4-147">なし</span><span class="sxs-lookup"><span data-stu-id="cbed4-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cbed4-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cbed4-148">JSON Representation</span></span>
<span data-ttu-id="cbed4-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cbed4-149">Here is a JSON representation of the resource.</span></span>
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



