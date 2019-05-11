---
title: deviceComplianceActionItem リソース タイプ
description: スケジュール済みのアクションの構成
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae816f98c4f570c1ab0c72063c7d15ad29054fae
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947184"
---
# <a name="devicecomplianceactionitem-resource-type"></a><span data-ttu-id="f4b27-103">deviceComplianceActionItem リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="f4b27-103">deviceComplianceActionItem resource type</span></span>

> <span data-ttu-id="f4b27-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4b27-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4b27-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f4b27-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4b27-106">スケジュール済みのアクションの構成</span><span class="sxs-lookup"><span data-stu-id="f4b27-106">Scheduled Action Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="f4b27-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="f4b27-107">Methods</span></span>
|<span data-ttu-id="f4b27-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="f4b27-108">Method</span></span>|<span data-ttu-id="f4b27-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f4b27-109">Return Type</span></span>|<span data-ttu-id="f4b27-110">説明</span><span class="sxs-lookup"><span data-stu-id="f4b27-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f4b27-111">List deviceComplianceActionItems</span><span class="sxs-lookup"><span data-stu-id="f4b27-111">List deviceComplianceActionItems</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-list.md)|<span data-ttu-id="f4b27-112">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f4b27-112">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) collection</span></span>|<span data-ttu-id="f4b27-113">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="f4b27-113">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>|
|[<span data-ttu-id="f4b27-114">Get deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="f4b27-114">Get deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-get.md)|[<span data-ttu-id="f4b27-115">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="f4b27-115">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="f4b27-116">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f4b27-116">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="f4b27-117">Create deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="f4b27-117">Create deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-create.md)|[<span data-ttu-id="f4b27-118">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="f4b27-118">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="f4b27-119">新しい [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f4b27-119">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="f4b27-120">Delete deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="f4b27-120">Delete deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-delete.md)|<span data-ttu-id="f4b27-121">なし</span><span class="sxs-lookup"><span data-stu-id="f4b27-121">None</span></span>|<span data-ttu-id="f4b27-122">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="f4b27-122">Deletes a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>|
|[<span data-ttu-id="f4b27-123">Update deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="f4b27-123">Update deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-update.md)|[<span data-ttu-id="f4b27-124">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="f4b27-124">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="f4b27-125">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f4b27-125">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f4b27-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4b27-126">Properties</span></span>
|<span data-ttu-id="f4b27-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4b27-127">Property</span></span>|<span data-ttu-id="f4b27-128">型</span><span class="sxs-lookup"><span data-stu-id="f4b27-128">Type</span></span>|<span data-ttu-id="f4b27-129">説明</span><span class="sxs-lookup"><span data-stu-id="f4b27-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4b27-130">id</span><span class="sxs-lookup"><span data-stu-id="f4b27-130">id</span></span>|<span data-ttu-id="f4b27-131">String</span><span class="sxs-lookup"><span data-stu-id="f4b27-131">String</span></span>|<span data-ttu-id="f4b27-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f4b27-132">Key of the entity.</span></span>|
|<span data-ttu-id="f4b27-133">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="f4b27-133">gracePeriodHours</span></span>|<span data-ttu-id="f4b27-134">Int32</span><span class="sxs-lookup"><span data-stu-id="f4b27-134">Int32</span></span>|<span data-ttu-id="f4b27-135">アクションが実行されるまでの待機時間。</span><span class="sxs-lookup"><span data-stu-id="f4b27-135">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="f4b27-136">有効な値は 0 から 8760 までです</span><span class="sxs-lookup"><span data-stu-id="f4b27-136">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="f4b27-137">actionType</span><span class="sxs-lookup"><span data-stu-id="f4b27-137">actionType</span></span>|[<span data-ttu-id="f4b27-138">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="f4b27-138">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="f4b27-139">実行するアクション。</span><span class="sxs-lookup"><span data-stu-id="f4b27-139">What action to take.</span></span> <span data-ttu-id="f4b27-140">可能な値は、`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock` です。</span><span class="sxs-lookup"><span data-stu-id="f4b27-140">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="f4b27-141">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="f4b27-141">notificationTemplateId</span></span>|<span data-ttu-id="f4b27-142">String</span><span class="sxs-lookup"><span data-stu-id="f4b27-142">String</span></span>|<span data-ttu-id="f4b27-143">使用する通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="f4b27-143">What notification Message template to use</span></span>|
|<span data-ttu-id="f4b27-144">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="f4b27-144">notificationMessageCCList</span></span>|<span data-ttu-id="f4b27-145">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f4b27-145">String collection</span></span>|<span data-ttu-id="f4b27-146">この通知メッセージの CC に設定するグループ ID のリスト。</span><span class="sxs-lookup"><span data-stu-id="f4b27-146">A list of group IDs to speicify who to CC this notification message to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4b27-147">関係</span><span class="sxs-lookup"><span data-stu-id="f4b27-147">Relationships</span></span>
<span data-ttu-id="f4b27-148">なし</span><span class="sxs-lookup"><span data-stu-id="f4b27-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4b27-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f4b27-149">JSON Representation</span></span>
<span data-ttu-id="f4b27-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f4b27-150">Here is a JSON representation of the resource.</span></span>
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




