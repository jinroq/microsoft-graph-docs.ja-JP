---
author: daspek
ms.author: dspektor
title: itemActivity リソースの種類
description: ItemActivity オブジェクトは、アイテムに対して行われたアクティビティに関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 98ae9e4881de18c94490469b10df43b2aaf58140
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536688"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="b190f-103">itemActivity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b190f-103">itemActivity resource type</span></span>

<span data-ttu-id="b190f-104">**Itemactivity**リソースは、アイテムまたはコンテナー内で行われたアクティビティに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="b190f-104">The **itemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="b190f-105">現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="b190f-105">Currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="b190f-106">ItemActivity 内で行われたアクションは、 [Itemactionset][]プロパティで詳細に説明されています。</span><span class="sxs-lookup"><span data-stu-id="b190f-106">The actions that took place within an itemActivity are detailed in the [itemActionSet][] property.</span></span>

><span data-ttu-id="b190f-107">**注:\*\*\*\*Itemactivity**は現在、SharePoint と OneDrive for business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="b190f-107">**Note:** **itemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActionSet]: itemactionset.md#properties

## <a name="properties"></a><span data-ttu-id="b190f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b190f-109">Properties</span></span>

| <span data-ttu-id="b190f-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b190f-110">Property</span></span> | <span data-ttu-id="b190f-111">型</span><span class="sxs-lookup"><span data-stu-id="b190f-111">Type</span></span>                    | <span data-ttu-id="b190f-112">説明</span><span class="sxs-lookup"><span data-stu-id="b190f-112">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="b190f-113">id</span><span class="sxs-lookup"><span data-stu-id="b190f-113">id</span></span>       | <span data-ttu-id="b190f-114">string</span><span class="sxs-lookup"><span data-stu-id="b190f-114">string</span></span>                  | <span data-ttu-id="b190f-115">アクティビティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="b190f-115">The unique identifier of the activity.</span></span> <span data-ttu-id="b190f-116">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b190f-116">Read-only.</span></span>
| <span data-ttu-id="b190f-117">接続</span><span class="sxs-lookup"><span data-stu-id="b190f-117">access</span></span>   | <span data-ttu-id="b190f-118">[accessAction][]</span><span class="sxs-lookup"><span data-stu-id="b190f-118">[accessAction][]</span></span>        | <span data-ttu-id="b190f-119">アイテムがアクセスされました。</span><span class="sxs-lookup"><span data-stu-id="b190f-119">An item was accessed.</span></span>
| <span data-ttu-id="b190f-120">actor</span><span class="sxs-lookup"><span data-stu-id="b190f-120">actor</span></span>    | <span data-ttu-id="b190f-121">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b190f-121">[identitySet][]</span></span>         | <span data-ttu-id="b190f-122">アクションを実行したユーザーの識別情報。</span><span class="sxs-lookup"><span data-stu-id="b190f-122">Identity of who performed the action.</span></span> <span data-ttu-id="b190f-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b190f-123">Read-only.</span></span>
| <span data-ttu-id="b190f-124">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="b190f-124">activityDateTime</span></span>    | <span data-ttu-id="b190f-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b190f-125">DateTimeOffset</span></span> | <span data-ttu-id="b190f-126">アクティビティがいつ発生したかについての詳細。</span><span class="sxs-lookup"><span data-stu-id="b190f-126">Details about when the activity took place.</span></span> <span data-ttu-id="b190f-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b190f-127">Read-only.</span></span>

[accessAction]: accessaction.md
[identitySet]: identityset.md

## <a name="relationships"></a><span data-ttu-id="b190f-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b190f-130">Relationships</span></span>

| <span data-ttu-id="b190f-131">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="b190f-131">Relationship name</span></span> | <span data-ttu-id="b190f-132">種類</span><span class="sxs-lookup"><span data-stu-id="b190f-132">Type</span></span>          | <span data-ttu-id="b190f-133">説明</span><span class="sxs-lookup"><span data-stu-id="b190f-133">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="b190f-134">driveItem</span><span class="sxs-lookup"><span data-stu-id="b190f-134">driveItem</span></span>         | <span data-ttu-id="b190f-135">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="b190f-135">[driveItem][]</span></span> | <span data-ttu-id="b190f-136">このアクティビティのターゲットとなった **driveItem** を表します。</span><span class="sxs-lookup"><span data-stu-id="b190f-136">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="b190f-137">listItem</span><span class="sxs-lookup"><span data-stu-id="b190f-137">listItem</span></span>          | <span data-ttu-id="b190f-138">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="b190f-138">[listItem][]</span></span>  | <span data-ttu-id="b190f-139">このアクティビティのターゲットとなった **listItem** を表します。</span><span class="sxs-lookup"><span data-stu-id="b190f-139">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="b190f-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b190f-142">JSON representation</span></span>

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
