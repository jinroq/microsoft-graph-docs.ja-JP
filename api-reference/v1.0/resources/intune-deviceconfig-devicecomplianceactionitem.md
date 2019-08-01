---
title: deviceComplianceActionItem リソース タイプ
description: スケジュール済みのアクションの構成
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1858996a6d0e41b7dfa8a2a4854a33878e7e13c2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028533"
---
# <a name="devicecomplianceactionitem-resource-type"></a><span data-ttu-id="35c81-103">deviceComplianceActionItem リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="35c81-103">deviceComplianceActionItem resource type</span></span>

> <span data-ttu-id="35c81-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="35c81-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35c81-105">スケジュール済みのアクションの構成</span><span class="sxs-lookup"><span data-stu-id="35c81-105">Scheduled Action Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="35c81-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="35c81-106">Methods</span></span>
|<span data-ttu-id="35c81-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="35c81-107">Method</span></span>|<span data-ttu-id="35c81-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="35c81-108">Return Type</span></span>|<span data-ttu-id="35c81-109">説明</span><span class="sxs-lookup"><span data-stu-id="35c81-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="35c81-110">List deviceComplianceActionItems</span><span class="sxs-lookup"><span data-stu-id="35c81-110">List deviceComplianceActionItems</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-list.md)|<span data-ttu-id="35c81-111">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="35c81-111">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) collection</span></span>|<span data-ttu-id="35c81-112">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="35c81-112">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>|
|[<span data-ttu-id="35c81-113">Get deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="35c81-113">Get deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-get.md)|[<span data-ttu-id="35c81-114">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="35c81-114">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="35c81-115">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="35c81-115">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="35c81-116">Create deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="35c81-116">Create deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-create.md)|[<span data-ttu-id="35c81-117">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="35c81-117">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="35c81-118">新しい [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="35c81-118">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="35c81-119">Delete deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="35c81-119">Delete deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-delete.md)|<span data-ttu-id="35c81-120">なし</span><span class="sxs-lookup"><span data-stu-id="35c81-120">None</span></span>|<span data-ttu-id="35c81-121">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="35c81-121">Deletes a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>|
|[<span data-ttu-id="35c81-122">Update deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="35c81-122">Update deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-update.md)|[<span data-ttu-id="35c81-123">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="35c81-123">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="35c81-124">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="35c81-124">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="35c81-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35c81-125">Properties</span></span>
|<span data-ttu-id="35c81-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35c81-126">Property</span></span>|<span data-ttu-id="35c81-127">型</span><span class="sxs-lookup"><span data-stu-id="35c81-127">Type</span></span>|<span data-ttu-id="35c81-128">説明</span><span class="sxs-lookup"><span data-stu-id="35c81-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35c81-129">id</span><span class="sxs-lookup"><span data-stu-id="35c81-129">id</span></span>|<span data-ttu-id="35c81-130">String</span><span class="sxs-lookup"><span data-stu-id="35c81-130">String</span></span>|<span data-ttu-id="35c81-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="35c81-131">Key of the entity.</span></span>|
|<span data-ttu-id="35c81-132">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="35c81-132">gracePeriodHours</span></span>|<span data-ttu-id="35c81-133">Int32</span><span class="sxs-lookup"><span data-stu-id="35c81-133">Int32</span></span>|<span data-ttu-id="35c81-134">アクションが実行されるまでの待機時間。</span><span class="sxs-lookup"><span data-stu-id="35c81-134">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="35c81-135">有効な値は 0 から 8760 までです</span><span class="sxs-lookup"><span data-stu-id="35c81-135">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="35c81-136">actionType</span><span class="sxs-lookup"><span data-stu-id="35c81-136">actionType</span></span>|[<span data-ttu-id="35c81-137">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="35c81-137">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="35c81-138">実行するアクション。</span><span class="sxs-lookup"><span data-stu-id="35c81-138">What action to take.</span></span> <span data-ttu-id="35c81-139">可能な値は、`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification` です。</span><span class="sxs-lookup"><span data-stu-id="35c81-139">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="35c81-140">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="35c81-140">notificationTemplateId</span></span>|<span data-ttu-id="35c81-141">String</span><span class="sxs-lookup"><span data-stu-id="35c81-141">String</span></span>|<span data-ttu-id="35c81-142">使用する通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="35c81-142">What notification Message template to use</span></span>|
|<span data-ttu-id="35c81-143">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="35c81-143">notificationMessageCCList</span></span>|<span data-ttu-id="35c81-144">String コレクション</span><span class="sxs-lookup"><span data-stu-id="35c81-144">String collection</span></span>|<span data-ttu-id="35c81-145">この通知メッセージの CC に設定するグループ ID のリスト。</span><span class="sxs-lookup"><span data-stu-id="35c81-145">A list of group IDs to speicify who to CC this notification message to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35c81-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="35c81-146">Relationships</span></span>
<span data-ttu-id="35c81-147">なし</span><span class="sxs-lookup"><span data-stu-id="35c81-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35c81-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="35c81-148">JSON Representation</span></span>
<span data-ttu-id="35c81-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="35c81-149">Here is a JSON representation of the resource.</span></span>
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



