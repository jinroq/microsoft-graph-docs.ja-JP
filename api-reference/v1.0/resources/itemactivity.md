---
author: daspek
ms.author: dspektor
title: itemActivity リソースの種類
description: ItemActivity オブジェクトは、アイテムに対して行われたアクティビティに関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c05493ddeb8e007da6ba8b7508369b4d013e672
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970757"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="b2913-103">itemActivity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b2913-103">itemActivity resource type</span></span>

<span data-ttu-id="b2913-104">**Itemactivity**リソースは、アイテムまたはコンテナー内で行われたアクティビティに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="b2913-104">The **itemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="b2913-105">現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="b2913-105">Currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="b2913-106">ItemActivity 内で行われたアクションは、 [Itemactionset][]プロパティで詳細に説明されています。</span><span class="sxs-lookup"><span data-stu-id="b2913-106">The actions that took place within an itemActivity are detailed in the [itemActionSet][] property.</span></span>

><span data-ttu-id="b2913-107">**注:\*\*\*\*Itemactivity**は現在、SharePoint と OneDrive for business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="b2913-107">**Note:** **itemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActionSet]: itemactionset.md#properties

## <a name="properties"></a><span data-ttu-id="b2913-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2913-109">Properties</span></span>

| <span data-ttu-id="b2913-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2913-110">Property</span></span> | <span data-ttu-id="b2913-111">型</span><span class="sxs-lookup"><span data-stu-id="b2913-111">Type</span></span>                    | <span data-ttu-id="b2913-112">説明</span><span class="sxs-lookup"><span data-stu-id="b2913-112">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="b2913-113">ID</span><span class="sxs-lookup"><span data-stu-id="b2913-113">id</span></span>       | <span data-ttu-id="b2913-114">string</span><span class="sxs-lookup"><span data-stu-id="b2913-114">string</span></span>                  | <span data-ttu-id="b2913-115">アクティビティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="b2913-115">The unique identifier of the activity.</span></span> <span data-ttu-id="b2913-116">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="b2913-116">Read-only.</span></span>
| <span data-ttu-id="b2913-117">接続</span><span class="sxs-lookup"><span data-stu-id="b2913-117">access</span></span>   | <span data-ttu-id="b2913-118">[accessAction][]</span><span class="sxs-lookup"><span data-stu-id="b2913-118">[accessAction][]</span></span>        | <span data-ttu-id="b2913-119">アイテムがアクセスされました。</span><span class="sxs-lookup"><span data-stu-id="b2913-119">An item was accessed.</span></span>
| <span data-ttu-id="b2913-120">actor</span><span class="sxs-lookup"><span data-stu-id="b2913-120">actor</span></span>    | <span data-ttu-id="b2913-121">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b2913-121">[identitySet][]</span></span>         | <span data-ttu-id="b2913-122">アクションを実行したユーザーの識別情報。</span><span class="sxs-lookup"><span data-stu-id="b2913-122">Identity of who performed the action.</span></span> <span data-ttu-id="b2913-123">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="b2913-123">Read-only.</span></span>
| <span data-ttu-id="b2913-124">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="b2913-124">activityDateTime</span></span>    | <span data-ttu-id="b2913-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2913-125">DateTimeOffset</span></span> | <span data-ttu-id="b2913-126">アクティビティがいつ発生したかについての詳細。</span><span class="sxs-lookup"><span data-stu-id="b2913-126">Details about when the activity took place.</span></span> <span data-ttu-id="b2913-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b2913-127">Read-only.</span></span>

[accessAction]: accessAction.md
[identitySet]: identityset.md

## <a name="relationships"></a><span data-ttu-id="b2913-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b2913-130">Relationships</span></span>

| <span data-ttu-id="b2913-131">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="b2913-131">Relationship name</span></span> | <span data-ttu-id="b2913-132">種類</span><span class="sxs-lookup"><span data-stu-id="b2913-132">Type</span></span>          | <span data-ttu-id="b2913-133">説明</span><span class="sxs-lookup"><span data-stu-id="b2913-133">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="b2913-134">driveItem</span><span class="sxs-lookup"><span data-stu-id="b2913-134">driveItem</span></span>         | <span data-ttu-id="b2913-135">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="b2913-135">[driveItem][]</span></span> | <span data-ttu-id="b2913-136">このアクティビティのターゲットとなった **driveItem** を表します。</span><span class="sxs-lookup"><span data-stu-id="b2913-136">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="b2913-137">listItem</span><span class="sxs-lookup"><span data-stu-id="b2913-137">listItem</span></span>          | <span data-ttu-id="b2913-138">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="b2913-138">[listItem][]</span></span>  | <span data-ttu-id="b2913-139">このアクティビティのターゲットとなった **listItem** を表します。</span><span class="sxs-lookup"><span data-stu-id="b2913-139">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="b2913-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b2913-142">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActivity",
  "@type.aka": "oneDrive.activityEntity"
}-->

```json
{
  "id": "string (identifier)",
  "access": "microsoft.graph.accessAction",
  "actor": {"@odata.type": "microsoft.graph.identitySet"},
  "driveItem": {"@odata.type": "microsoft.graph.driveItem"},
  "listItem": {"@odata.type": "microsoft.graph.listItem"},
  "activityDateTime": {"@odata.type": "String (timestamp)"}
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The itemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/itemActivity",
  "suppressions": []
}
-->
