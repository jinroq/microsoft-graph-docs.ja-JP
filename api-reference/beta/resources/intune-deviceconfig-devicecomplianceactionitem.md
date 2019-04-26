---
title: deviceComplianceActionItem リソース タイプ
description: スケジュール済みのアクションの構成
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 44a69bc11c18323df7ebf1932d75df762dbc0872
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561293"
---
# <a name="devicecomplianceactionitem-resource-type"></a><span data-ttu-id="4dc6d-103">deviceComplianceActionItem リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="4dc6d-103">deviceComplianceActionItem resource type</span></span>

> <span data-ttu-id="4dc6d-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4dc6d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4dc6d-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4dc6d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4dc6d-106">スケジュール済みのアクションの構成</span><span class="sxs-lookup"><span data-stu-id="4dc6d-106">Scheduled Action Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="4dc6d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="4dc6d-107">Methods</span></span>
|<span data-ttu-id="4dc6d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="4dc6d-108">Method</span></span>|<span data-ttu-id="4dc6d-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4dc6d-109">Return Type</span></span>|<span data-ttu-id="4dc6d-110">説明</span><span class="sxs-lookup"><span data-stu-id="4dc6d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4dc6d-111">List deviceComplianceActionItems</span><span class="sxs-lookup"><span data-stu-id="4dc6d-111">List deviceComplianceActionItems</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-list.md)|<span data-ttu-id="4dc6d-112">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4dc6d-112">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) collection</span></span>|<span data-ttu-id="4dc6d-113">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="4dc6d-113">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>|
|[<span data-ttu-id="4dc6d-114">Get deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="4dc6d-114">Get deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-get.md)|[<span data-ttu-id="4dc6d-115">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="4dc6d-115">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="4dc6d-116">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4dc6d-116">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="4dc6d-117">Create deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="4dc6d-117">Create deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-create.md)|[<span data-ttu-id="4dc6d-118">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="4dc6d-118">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="4dc6d-119">新しい [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4dc6d-119">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="4dc6d-120">Delete deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="4dc6d-120">Delete deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-delete.md)|<span data-ttu-id="4dc6d-121">なし</span><span class="sxs-lookup"><span data-stu-id="4dc6d-121">None</span></span>|<span data-ttu-id="4dc6d-122">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="4dc6d-122">Deletes a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>|
|[<span data-ttu-id="4dc6d-123">Update deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="4dc6d-123">Update deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-update.md)|[<span data-ttu-id="4dc6d-124">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="4dc6d-124">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="4dc6d-125">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4dc6d-125">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4dc6d-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4dc6d-126">Properties</span></span>
|<span data-ttu-id="4dc6d-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4dc6d-127">Property</span></span>|<span data-ttu-id="4dc6d-128">型</span><span class="sxs-lookup"><span data-stu-id="4dc6d-128">Type</span></span>|<span data-ttu-id="4dc6d-129">説明</span><span class="sxs-lookup"><span data-stu-id="4dc6d-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dc6d-130">id</span><span class="sxs-lookup"><span data-stu-id="4dc6d-130">id</span></span>|<span data-ttu-id="4dc6d-131">String</span><span class="sxs-lookup"><span data-stu-id="4dc6d-131">String</span></span>|<span data-ttu-id="4dc6d-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4dc6d-132">Key of the entity.</span></span>|
|<span data-ttu-id="4dc6d-133">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="4dc6d-133">gracePeriodHours</span></span>|<span data-ttu-id="4dc6d-134">Int32</span><span class="sxs-lookup"><span data-stu-id="4dc6d-134">Int32</span></span>|<span data-ttu-id="4dc6d-135">アクションが実行されるまでの待機時間。</span><span class="sxs-lookup"><span data-stu-id="4dc6d-135">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="4dc6d-136">有効な値は 0 から 8760 までです</span><span class="sxs-lookup"><span data-stu-id="4dc6d-136">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="4dc6d-137">actionType</span><span class="sxs-lookup"><span data-stu-id="4dc6d-137">actionType</span></span>|[<span data-ttu-id="4dc6d-138">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="4dc6d-138">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="4dc6d-139">実行するアクション。</span><span class="sxs-lookup"><span data-stu-id="4dc6d-139">What action to take.</span></span> <span data-ttu-id="4dc6d-140">可能な値は、`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock` です。</span><span class="sxs-lookup"><span data-stu-id="4dc6d-140">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="4dc6d-141">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="4dc6d-141">notificationTemplateId</span></span>|<span data-ttu-id="4dc6d-142">String</span><span class="sxs-lookup"><span data-stu-id="4dc6d-142">String</span></span>|<span data-ttu-id="4dc6d-143">使用する通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="4dc6d-143">What notification Message template to use</span></span>|
|<span data-ttu-id="4dc6d-144">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="4dc6d-144">notificationMessageCCList</span></span>|<span data-ttu-id="4dc6d-145">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4dc6d-145">String collection</span></span>|<span data-ttu-id="4dc6d-146">この通知メッセージの CC に設定するグループ ID のリスト。</span><span class="sxs-lookup"><span data-stu-id="4dc6d-146">A list of group IDs to speicify who to CC this notification message to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4dc6d-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4dc6d-147">Relationships</span></span>
<span data-ttu-id="4dc6d-148">なし</span><span class="sxs-lookup"><span data-stu-id="4dc6d-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4dc6d-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4dc6d-149">JSON Representation</span></span>
<span data-ttu-id="4dc6d-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4dc6d-150">Here is a JSON representation of the resource.</span></span>
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





