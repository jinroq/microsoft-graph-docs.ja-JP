---
title: deviceComplianceActionItem リソース タイプ
description: スケジュール済みのアクションの構成
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6a96ca90ee9967968799e2bc1bea281346eaf1c4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414964"
---
# <a name="devicecomplianceactionitem-resource-type"></a><span data-ttu-id="deda3-103">deviceComplianceActionItem リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="deda3-103">deviceComplianceActionItem resource type</span></span>

> <span data-ttu-id="deda3-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="deda3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="deda3-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="deda3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="deda3-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="deda3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="deda3-107">スケジュール済みのアクションの構成</span><span class="sxs-lookup"><span data-stu-id="deda3-107">Scheduled Action Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="deda3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="deda3-108">Methods</span></span>
|<span data-ttu-id="deda3-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="deda3-109">Method</span></span>|<span data-ttu-id="deda3-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="deda3-110">Return Type</span></span>|<span data-ttu-id="deda3-111">説明</span><span class="sxs-lookup"><span data-stu-id="deda3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="deda3-112">List deviceComplianceActionItems</span><span class="sxs-lookup"><span data-stu-id="deda3-112">List deviceComplianceActionItems</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-list.md)|<span data-ttu-id="deda3-113">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="deda3-113">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) collection</span></span>|<span data-ttu-id="deda3-114">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="deda3-114">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>|
|[<span data-ttu-id="deda3-115">Get deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="deda3-115">Get deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-get.md)|[<span data-ttu-id="deda3-116">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="deda3-116">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="deda3-117">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="deda3-117">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="deda3-118">Create deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="deda3-118">Create deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-create.md)|[<span data-ttu-id="deda3-119">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="deda3-119">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="deda3-120">新しい [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="deda3-120">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="deda3-121">Delete deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="deda3-121">Delete deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-delete.md)|<span data-ttu-id="deda3-122">なし</span><span class="sxs-lookup"><span data-stu-id="deda3-122">None</span></span>|<span data-ttu-id="deda3-123">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="deda3-123">Deletes a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>|
|[<span data-ttu-id="deda3-124">Update deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="deda3-124">Update deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-update.md)|[<span data-ttu-id="deda3-125">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="deda3-125">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="deda3-126">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="deda3-126">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="deda3-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="deda3-127">Properties</span></span>
|<span data-ttu-id="deda3-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="deda3-128">Property</span></span>|<span data-ttu-id="deda3-129">型</span><span class="sxs-lookup"><span data-stu-id="deda3-129">Type</span></span>|<span data-ttu-id="deda3-130">説明</span><span class="sxs-lookup"><span data-stu-id="deda3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="deda3-131">id</span><span class="sxs-lookup"><span data-stu-id="deda3-131">id</span></span>|<span data-ttu-id="deda3-132">String</span><span class="sxs-lookup"><span data-stu-id="deda3-132">String</span></span>|<span data-ttu-id="deda3-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="deda3-133">Key of the entity.</span></span>|
|<span data-ttu-id="deda3-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="deda3-134">gracePeriodHours</span></span>|<span data-ttu-id="deda3-135">Int32</span><span class="sxs-lookup"><span data-stu-id="deda3-135">Int32</span></span>|<span data-ttu-id="deda3-136">アクションが実行されるまでの待機時間。</span><span class="sxs-lookup"><span data-stu-id="deda3-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="deda3-137">有効な値は 0 から 8760 までです</span><span class="sxs-lookup"><span data-stu-id="deda3-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="deda3-138">actionType</span><span class="sxs-lookup"><span data-stu-id="deda3-138">actionType</span></span>|[<span data-ttu-id="deda3-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="deda3-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="deda3-140">実行するアクションです。</span><span class="sxs-lookup"><span data-stu-id="deda3-140">What action to take.</span></span> <span data-ttu-id="deda3-141">可能な値は、`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock` です。</span><span class="sxs-lookup"><span data-stu-id="deda3-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="deda3-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="deda3-142">notificationTemplateId</span></span>|<span data-ttu-id="deda3-143">String</span><span class="sxs-lookup"><span data-stu-id="deda3-143">String</span></span>|<span data-ttu-id="deda3-144">使用する通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="deda3-144">What notification Message template to use</span></span>|
|<span data-ttu-id="deda3-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="deda3-145">notificationMessageCCList</span></span>|<span data-ttu-id="deda3-146">String コレクション</span><span class="sxs-lookup"><span data-stu-id="deda3-146">String collection</span></span>|<span data-ttu-id="deda3-147">この通知メッセージの CC に設定するグループ ID のリスト。</span><span class="sxs-lookup"><span data-stu-id="deda3-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="deda3-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="deda3-148">Relationships</span></span>
<span data-ttu-id="deda3-149">なし</span><span class="sxs-lookup"><span data-stu-id="deda3-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="deda3-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="deda3-150">JSON Representation</span></span>
<span data-ttu-id="deda3-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="deda3-151">Here is a JSON representation of the resource.</span></span>
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




