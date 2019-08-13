---
title: deviceComplianceActionItem リソース タイプ
description: スケジュール済みのアクションの構成
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c4a8e58d083f0985164d34607a9b7970025dee1e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333227"
---
# <a name="devicecomplianceactionitem-resource-type"></a><span data-ttu-id="aa532-103">deviceComplianceActionItem リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="aa532-103">deviceComplianceActionItem resource type</span></span>

> <span data-ttu-id="aa532-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa532-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa532-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="aa532-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa532-106">スケジュール済みのアクションの構成</span><span class="sxs-lookup"><span data-stu-id="aa532-106">Scheduled Action Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="aa532-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="aa532-107">Methods</span></span>
|<span data-ttu-id="aa532-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="aa532-108">Method</span></span>|<span data-ttu-id="aa532-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="aa532-109">Return Type</span></span>|<span data-ttu-id="aa532-110">説明</span><span class="sxs-lookup"><span data-stu-id="aa532-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aa532-111">List deviceComplianceActionItems</span><span class="sxs-lookup"><span data-stu-id="aa532-111">List deviceComplianceActionItems</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-list.md)|<span data-ttu-id="aa532-112">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="aa532-112">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) collection</span></span>|<span data-ttu-id="aa532-113">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="aa532-113">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>|
|[<span data-ttu-id="aa532-114">Get deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="aa532-114">Get deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-get.md)|[<span data-ttu-id="aa532-115">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="aa532-115">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="aa532-116">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="aa532-116">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="aa532-117">Create deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="aa532-117">Create deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-create.md)|[<span data-ttu-id="aa532-118">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="aa532-118">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="aa532-119">新しい [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="aa532-119">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="aa532-120">Delete deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="aa532-120">Delete deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-delete.md)|<span data-ttu-id="aa532-121">なし</span><span class="sxs-lookup"><span data-stu-id="aa532-121">None</span></span>|<span data-ttu-id="aa532-122">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="aa532-122">Deletes a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>|
|[<span data-ttu-id="aa532-123">Update deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="aa532-123">Update deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-update.md)|[<span data-ttu-id="aa532-124">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="aa532-124">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="aa532-125">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="aa532-125">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aa532-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa532-126">Properties</span></span>
|<span data-ttu-id="aa532-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa532-127">Property</span></span>|<span data-ttu-id="aa532-128">型</span><span class="sxs-lookup"><span data-stu-id="aa532-128">Type</span></span>|<span data-ttu-id="aa532-129">説明</span><span class="sxs-lookup"><span data-stu-id="aa532-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa532-130">id</span><span class="sxs-lookup"><span data-stu-id="aa532-130">id</span></span>|<span data-ttu-id="aa532-131">String</span><span class="sxs-lookup"><span data-stu-id="aa532-131">String</span></span>|<span data-ttu-id="aa532-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="aa532-132">Key of the entity.</span></span>|
|<span data-ttu-id="aa532-133">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="aa532-133">gracePeriodHours</span></span>|<span data-ttu-id="aa532-134">Int32</span><span class="sxs-lookup"><span data-stu-id="aa532-134">Int32</span></span>|<span data-ttu-id="aa532-135">アクションが実行されるまでの待機時間。</span><span class="sxs-lookup"><span data-stu-id="aa532-135">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="aa532-136">有効な値は 0 から 8760 までです</span><span class="sxs-lookup"><span data-stu-id="aa532-136">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="aa532-137">actionType</span><span class="sxs-lookup"><span data-stu-id="aa532-137">actionType</span></span>|[<span data-ttu-id="aa532-138">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="aa532-138">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="aa532-139">実行するアクション。</span><span class="sxs-lookup"><span data-stu-id="aa532-139">What action to take.</span></span> <span data-ttu-id="aa532-140">可能な値は、`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock` です。</span><span class="sxs-lookup"><span data-stu-id="aa532-140">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="aa532-141">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="aa532-141">notificationTemplateId</span></span>|<span data-ttu-id="aa532-142">String</span><span class="sxs-lookup"><span data-stu-id="aa532-142">String</span></span>|<span data-ttu-id="aa532-143">使用する通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="aa532-143">What notification Message template to use</span></span>|
|<span data-ttu-id="aa532-144">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="aa532-144">notificationMessageCCList</span></span>|<span data-ttu-id="aa532-145">String コレクション</span><span class="sxs-lookup"><span data-stu-id="aa532-145">String collection</span></span>|<span data-ttu-id="aa532-146">この通知メッセージの CC に設定するグループ ID のリスト。</span><span class="sxs-lookup"><span data-stu-id="aa532-146">A list of group IDs to speicify who to CC this notification message to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa532-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aa532-147">Relationships</span></span>
<span data-ttu-id="aa532-148">なし</span><span class="sxs-lookup"><span data-stu-id="aa532-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa532-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aa532-149">JSON Representation</span></span>
<span data-ttu-id="aa532-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aa532-150">Here is a JSON representation of the resource.</span></span>
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



