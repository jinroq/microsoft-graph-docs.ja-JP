---
title: deviceComplianceActionItem リソース タイプ
description: スケジュール済みのアクションの構成
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0676acc44946b327772083ccd6e46e3f47df648f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980196"
---
# <a name="devicecomplianceactionitem-resource-type"></a><span data-ttu-id="45c61-103">deviceComplianceActionItem リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="45c61-103">deviceComplianceActionItem resource type</span></span>

> <span data-ttu-id="45c61-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="45c61-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45c61-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45c61-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45c61-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="45c61-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45c61-107">スケジュール済みのアクションの構成</span><span class="sxs-lookup"><span data-stu-id="45c61-107">Scheduled Action Configuration</span></span>
## <a name="methods"></a><span data-ttu-id="45c61-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="45c61-108">Methods</span></span>
|<span data-ttu-id="45c61-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="45c61-109">Method</span></span>|<span data-ttu-id="45c61-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="45c61-110">Return Type</span></span>|<span data-ttu-id="45c61-111">説明</span><span class="sxs-lookup"><span data-stu-id="45c61-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="45c61-112">List deviceComplianceActionItems</span><span class="sxs-lookup"><span data-stu-id="45c61-112">List deviceComplianceActionItems</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-list.md)|<span data-ttu-id="45c61-113">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="45c61-113">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) collection</span></span>|<span data-ttu-id="45c61-114">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="45c61-114">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>|
|[<span data-ttu-id="45c61-115">Get deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="45c61-115">Get deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-get.md)|[<span data-ttu-id="45c61-116">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="45c61-116">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="45c61-117">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="45c61-117">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="45c61-118">Create deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="45c61-118">Create deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-create.md)|[<span data-ttu-id="45c61-119">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="45c61-119">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="45c61-120">新しい [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="45c61-120">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="45c61-121">Delete deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="45c61-121">Delete deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-delete.md)|<span data-ttu-id="45c61-122">なし</span><span class="sxs-lookup"><span data-stu-id="45c61-122">None</span></span>|<span data-ttu-id="45c61-123">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="45c61-123">Deletes a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>|
|[<span data-ttu-id="45c61-124">Update deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="45c61-124">Update deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-update.md)|[<span data-ttu-id="45c61-125">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="45c61-125">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="45c61-126">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="45c61-126">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="45c61-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45c61-127">Properties</span></span>
|<span data-ttu-id="45c61-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45c61-128">Property</span></span>|<span data-ttu-id="45c61-129">型</span><span class="sxs-lookup"><span data-stu-id="45c61-129">Type</span></span>|<span data-ttu-id="45c61-130">説明</span><span class="sxs-lookup"><span data-stu-id="45c61-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45c61-131">ID</span><span class="sxs-lookup"><span data-stu-id="45c61-131">id</span></span>|<span data-ttu-id="45c61-132">String</span><span class="sxs-lookup"><span data-stu-id="45c61-132">String</span></span>|<span data-ttu-id="45c61-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="45c61-133">Key of the entity.</span></span>|
|<span data-ttu-id="45c61-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="45c61-134">gracePeriodHours</span></span>|<span data-ttu-id="45c61-135">Int32</span><span class="sxs-lookup"><span data-stu-id="45c61-135">Int32</span></span>|<span data-ttu-id="45c61-136">アクションが実行されるまでの待機時間。</span><span class="sxs-lookup"><span data-stu-id="45c61-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="45c61-137">有効な値は 0 から 8760 までです</span><span class="sxs-lookup"><span data-stu-id="45c61-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="45c61-138">actionType</span><span class="sxs-lookup"><span data-stu-id="45c61-138">actionType</span></span>|[<span data-ttu-id="45c61-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="45c61-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="45c61-140">実行するアクションです。</span><span class="sxs-lookup"><span data-stu-id="45c61-140">What action to take.</span></span> <span data-ttu-id="45c61-141">可能な値は、`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock` です。</span><span class="sxs-lookup"><span data-stu-id="45c61-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="45c61-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="45c61-142">notificationTemplateId</span></span>|<span data-ttu-id="45c61-143">String</span><span class="sxs-lookup"><span data-stu-id="45c61-143">String</span></span>|<span data-ttu-id="45c61-144">使用する通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="45c61-144">What notification Message template to use</span></span>|
|<span data-ttu-id="45c61-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="45c61-145">notificationMessageCCList</span></span>|<span data-ttu-id="45c61-146">String コレクション</span><span class="sxs-lookup"><span data-stu-id="45c61-146">String collection</span></span>|<span data-ttu-id="45c61-147">この通知メッセージの CC に設定するグループ ID のリスト。</span><span class="sxs-lookup"><span data-stu-id="45c61-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45c61-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="45c61-148">Relationships</span></span>
<span data-ttu-id="45c61-149">なし</span><span class="sxs-lookup"><span data-stu-id="45c61-149">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="45c61-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="45c61-150">JSON Representation</span></span>
<span data-ttu-id="45c61-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="45c61-151">Here is a JSON representation of the resource.</span></span>
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





