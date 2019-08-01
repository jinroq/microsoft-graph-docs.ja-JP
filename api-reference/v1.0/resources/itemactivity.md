---
author: daspek
ms.author: dspektor
title: itemActivity リソースの種類
description: ItemActivity オブジェクトは、アイテムに対して行われたアクティビティに関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: ddd478794cc3ad87ce29513c45455a9ba2911a52
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036730"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="9967b-103">itemActivity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9967b-103">itemActivity resource type</span></span>

<span data-ttu-id="9967b-104">**Itemactivity**リソースは、アイテムまたはコンテナー内で行われたアクティビティに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="9967b-104">The **itemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="9967b-105">現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="9967b-105">Currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="9967b-106">ItemActivity 内で行われたアクションは、 [Itemactionset][]プロパティで詳細に説明されています。</span><span class="sxs-lookup"><span data-stu-id="9967b-106">The actions that took place within an itemActivity are detailed in the [itemActionSet][] property.</span></span>

><span data-ttu-id="9967b-107">**注:\*\*\*\*Itemactivity**は現在、SharePoint と OneDrive for business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="9967b-107">**Note:** **itemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActionSet]: itemactionset.md#properties

## <a name="properties"></a><span data-ttu-id="9967b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9967b-109">Properties</span></span>

| <span data-ttu-id="9967b-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9967b-110">Property</span></span> | <span data-ttu-id="9967b-111">型</span><span class="sxs-lookup"><span data-stu-id="9967b-111">Type</span></span>                    | <span data-ttu-id="9967b-112">説明</span><span class="sxs-lookup"><span data-stu-id="9967b-112">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="9967b-113">id</span><span class="sxs-lookup"><span data-stu-id="9967b-113">id</span></span>       | <span data-ttu-id="9967b-114">string</span><span class="sxs-lookup"><span data-stu-id="9967b-114">string</span></span>                  | <span data-ttu-id="9967b-115">アクティビティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="9967b-115">The unique identifier of the activity.</span></span> <span data-ttu-id="9967b-116">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9967b-116">Read-only.</span></span>
| <span data-ttu-id="9967b-117">接続</span><span class="sxs-lookup"><span data-stu-id="9967b-117">access</span></span>   | <span data-ttu-id="9967b-118">[accessAction][]</span><span class="sxs-lookup"><span data-stu-id="9967b-118">[accessAction][]</span></span>        | <span data-ttu-id="9967b-119">アイテムがアクセスされました。</span><span class="sxs-lookup"><span data-stu-id="9967b-119">An item was accessed.</span></span>
| <span data-ttu-id="9967b-120">actor</span><span class="sxs-lookup"><span data-stu-id="9967b-120">actor</span></span>    | <span data-ttu-id="9967b-121">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="9967b-121">[identitySet][]</span></span>         | <span data-ttu-id="9967b-122">アクションを実行したユーザーの識別情報。</span><span class="sxs-lookup"><span data-stu-id="9967b-122">Identity of who performed the action.</span></span> <span data-ttu-id="9967b-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9967b-123">Read-only.</span></span>
| <span data-ttu-id="9967b-124">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="9967b-124">activityDateTime</span></span>    | <span data-ttu-id="9967b-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9967b-125">DateTimeOffset</span></span> | <span data-ttu-id="9967b-126">アクティビティがいつ発生したかについての詳細。</span><span class="sxs-lookup"><span data-stu-id="9967b-126">Details about when the activity took place.</span></span> <span data-ttu-id="9967b-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9967b-127">Read-only.</span></span>

[accessAction]: accessaction.md
[identitySet]: identityset.md

## <a name="relationships"></a><span data-ttu-id="9967b-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9967b-130">Relationships</span></span>

| <span data-ttu-id="9967b-131">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="9967b-131">Relationship name</span></span> | <span data-ttu-id="9967b-132">種類</span><span class="sxs-lookup"><span data-stu-id="9967b-132">Type</span></span>          | <span data-ttu-id="9967b-133">説明</span><span class="sxs-lookup"><span data-stu-id="9967b-133">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="9967b-134">driveItem</span><span class="sxs-lookup"><span data-stu-id="9967b-134">driveItem</span></span>         | <span data-ttu-id="9967b-135">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="9967b-135">[driveItem][]</span></span> | <span data-ttu-id="9967b-136">このアクティビティのターゲットとなった **driveItem** を表します。</span><span class="sxs-lookup"><span data-stu-id="9967b-136">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="9967b-137">listItem</span><span class="sxs-lookup"><span data-stu-id="9967b-137">listItem</span></span>          | <span data-ttu-id="9967b-138">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="9967b-138">[listItem][]</span></span>  | <span data-ttu-id="9967b-139">このアクティビティのターゲットとなった **listItem** を表します。</span><span class="sxs-lookup"><span data-stu-id="9967b-139">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="9967b-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9967b-142">JSON representation</span></span>

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
