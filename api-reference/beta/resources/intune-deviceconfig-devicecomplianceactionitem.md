---
title: deviceComplianceActionItem リソース タイプ
description: スケジュール済みのアクションの構成
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d697275780b686edc9a3b1eed42b6afb712163b0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866431"
---
# <a name="devicecomplianceactionitem-resource-type"></a><span data-ttu-id="167a9-103">deviceComplianceActionItem リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="167a9-103">deviceComplianceActionItem resource type</span></span>

> <span data-ttu-id="167a9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="167a9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="167a9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="167a9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="167a9-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="167a9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="167a9-107">スケジュール済みのアクションの構成</span><span class="sxs-lookup"><span data-stu-id="167a9-107">Scheduled Action Configuration</span></span>
## <a name="methods"></a><span data-ttu-id="167a9-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="167a9-108">Methods</span></span>
|<span data-ttu-id="167a9-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="167a9-109">Method</span></span>|<span data-ttu-id="167a9-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="167a9-110">Return Type</span></span>|<span data-ttu-id="167a9-111">説明</span><span class="sxs-lookup"><span data-stu-id="167a9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="167a9-112">List deviceComplianceActionItems</span><span class="sxs-lookup"><span data-stu-id="167a9-112">List deviceComplianceActionItems</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-list.md)|<span data-ttu-id="167a9-113">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="167a9-113">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) collection</span></span>|<span data-ttu-id="167a9-114">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="167a9-114">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>|
|[<span data-ttu-id="167a9-115">Get deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="167a9-115">Get deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-get.md)|[<span data-ttu-id="167a9-116">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="167a9-116">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="167a9-117">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="167a9-117">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="167a9-118">Create deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="167a9-118">Create deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-create.md)|[<span data-ttu-id="167a9-119">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="167a9-119">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="167a9-120">新しい [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="167a9-120">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="167a9-121">Delete deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="167a9-121">Delete deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-delete.md)|<span data-ttu-id="167a9-122">なし</span><span class="sxs-lookup"><span data-stu-id="167a9-122">None</span></span>|<span data-ttu-id="167a9-123">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="167a9-123">Deletes a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>|
|[<span data-ttu-id="167a9-124">Update deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="167a9-124">Update deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-update.md)|[<span data-ttu-id="167a9-125">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="167a9-125">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="167a9-126">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="167a9-126">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="167a9-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="167a9-127">Properties</span></span>
|<span data-ttu-id="167a9-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="167a9-128">Property</span></span>|<span data-ttu-id="167a9-129">種類</span><span class="sxs-lookup"><span data-stu-id="167a9-129">Type</span></span>|<span data-ttu-id="167a9-130">説明</span><span class="sxs-lookup"><span data-stu-id="167a9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="167a9-131">ID</span><span class="sxs-lookup"><span data-stu-id="167a9-131">id</span></span>|<span data-ttu-id="167a9-132">String</span><span class="sxs-lookup"><span data-stu-id="167a9-132">String</span></span>|<span data-ttu-id="167a9-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="167a9-133">Key of the entity.</span></span>|
|<span data-ttu-id="167a9-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="167a9-134">gracePeriodHours</span></span>|<span data-ttu-id="167a9-135">Int32</span><span class="sxs-lookup"><span data-stu-id="167a9-135">Int32</span></span>|<span data-ttu-id="167a9-136">アクションが実行されるまでの待機時間。</span><span class="sxs-lookup"><span data-stu-id="167a9-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="167a9-137">有効な値は 0 から 8760 までです</span><span class="sxs-lookup"><span data-stu-id="167a9-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="167a9-138">actionType</span><span class="sxs-lookup"><span data-stu-id="167a9-138">actionType</span></span>|[<span data-ttu-id="167a9-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="167a9-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="167a9-140">実行するアクションです。</span><span class="sxs-lookup"><span data-stu-id="167a9-140">What action to take.</span></span> <span data-ttu-id="167a9-141">可能な値は、`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock` です。</span><span class="sxs-lookup"><span data-stu-id="167a9-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="167a9-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="167a9-142">notificationTemplateId</span></span>|<span data-ttu-id="167a9-143">String</span><span class="sxs-lookup"><span data-stu-id="167a9-143">String</span></span>|<span data-ttu-id="167a9-144">使用する通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="167a9-144">What notification Message template to use</span></span>|
|<span data-ttu-id="167a9-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="167a9-145">notificationMessageCCList</span></span>|<span data-ttu-id="167a9-146">String コレクション</span><span class="sxs-lookup"><span data-stu-id="167a9-146">String collection</span></span>|<span data-ttu-id="167a9-147">この通知メッセージの CC に設定するグループ ID のリスト。</span><span class="sxs-lookup"><span data-stu-id="167a9-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="167a9-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="167a9-148">Relationships</span></span>
<span data-ttu-id="167a9-149">なし</span><span class="sxs-lookup"><span data-stu-id="167a9-149">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="167a9-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="167a9-150">JSON Representation</span></span>
<span data-ttu-id="167a9-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="167a9-151">Here is a JSON representation of the resource.</span></span>
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





