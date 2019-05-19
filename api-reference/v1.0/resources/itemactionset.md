---
author: daspek
ms.author: dspektor
title: ItemActionSet リソースの種類
description: ItemActionSet オブジェクトは、アイテムのアクティビティの一部として行われたアクションに関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 065a6126e2e4a2f78cecfb2ae5497fac28e16899
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970759"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="c4878-103">itemActionSet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c4878-103">itemActionSet resource type</span></span>

<span data-ttu-id="c4878-104">**Itemactionset**リソースは、アイテムの[アクティビティ][ itemActivity]を構成したアクションに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="c4878-104">The **itemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

><span data-ttu-id="c4878-105">**注:** 現時点では、アイテムアクティビティレコードは SharePoint および OneDrive for business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="c4878-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActivity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="c4878-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4878-106">Properties</span></span>

<span data-ttu-id="c4878-107">現在、次の操作を実行できます。</span><span class="sxs-lookup"><span data-stu-id="c4878-107">The following actions are currently available.</span></span> <span data-ttu-id="c4878-108">今後、新しいアクションが追加される可能性があるため、アプリが不明なアクションを含む**Itemactionset**を処理できることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="c4878-108">Because new actions might be added in the future, make sure that your app can handle an **itemActionSet** that includes unknown actions.</span></span>

| <span data-ttu-id="c4878-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="c4878-109">Property name</span></span> | <span data-ttu-id="c4878-110">種類</span><span class="sxs-lookup"><span data-stu-id="c4878-110">Type</span></span>              | <span data-ttu-id="c4878-111">説明</span><span class="sxs-lookup"><span data-stu-id="c4878-111">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="c4878-112">comment</span><span class="sxs-lookup"><span data-stu-id="c4878-112">comment</span></span>       | <span data-ttu-id="c4878-113">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="c4878-113">[commentAction][]</span></span> | <span data-ttu-id="c4878-114">アイテムにコメントが追加されました。</span><span class="sxs-lookup"><span data-stu-id="c4878-114">A comment was added to the item.</span></span>
| <span data-ttu-id="c4878-115">create</span><span class="sxs-lookup"><span data-stu-id="c4878-115">create</span></span>        | <span data-ttu-id="c4878-116">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="c4878-116">[createAction][]</span></span>  | <span data-ttu-id="c4878-117">アイテムが作成されました。</span><span class="sxs-lookup"><span data-stu-id="c4878-117">An item was created.</span></span>
| <span data-ttu-id="c4878-118">delete</span><span class="sxs-lookup"><span data-stu-id="c4878-118">delete</span></span>        | <span data-ttu-id="c4878-119">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="c4878-119">[deleteAction][]</span></span>  | <span data-ttu-id="c4878-120">アイテムが削除されました。</span><span class="sxs-lookup"><span data-stu-id="c4878-120">An item was deleted.</span></span>
| <span data-ttu-id="c4878-121">edit</span><span class="sxs-lookup"><span data-stu-id="c4878-121">edit</span></span>          | <span data-ttu-id="c4878-122">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="c4878-122">[editAction][]</span></span>    | <span data-ttu-id="c4878-123">アイテムが編集されました。</span><span class="sxs-lookup"><span data-stu-id="c4878-123">An item was edited.</span></span>
| <span data-ttu-id="c4878-124">mention</span><span class="sxs-lookup"><span data-stu-id="c4878-124">mention</span></span>       | <span data-ttu-id="c4878-125">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="c4878-125">[mentionAction][]</span></span> | <span data-ttu-id="c4878-126">アイテムでユーザーがメンションされました。</span><span class="sxs-lookup"><span data-stu-id="c4878-126">A user was mentioned in the item.</span></span>
| <span data-ttu-id="c4878-127">move</span><span class="sxs-lookup"><span data-stu-id="c4878-127">move</span></span>          | <span data-ttu-id="c4878-128">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="c4878-128">[moveAction][]</span></span>    | <span data-ttu-id="c4878-129">アイテムが移動されました。</span><span class="sxs-lookup"><span data-stu-id="c4878-129">An item was moved.</span></span>
| <span data-ttu-id="c4878-130">rename</span><span class="sxs-lookup"><span data-stu-id="c4878-130">rename</span></span>        | <span data-ttu-id="c4878-131">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="c4878-131">[renameAction][]</span></span>  | <span data-ttu-id="c4878-132">アイテムの名前が変更されました。</span><span class="sxs-lookup"><span data-stu-id="c4878-132">An item was renamed.</span></span>
| <span data-ttu-id="c4878-133">restore</span><span class="sxs-lookup"><span data-stu-id="c4878-133">restore</span></span>       | <span data-ttu-id="c4878-134">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="c4878-134">[restoreAction][]</span></span> | <span data-ttu-id="c4878-135">アイテムが復元されました。</span><span class="sxs-lookup"><span data-stu-id="c4878-135">An item was restored.</span></span>
| <span data-ttu-id="c4878-136">share</span><span class="sxs-lookup"><span data-stu-id="c4878-136">share</span></span>         | <span data-ttu-id="c4878-137">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="c4878-137">[shareAction][]</span></span>   | <span data-ttu-id="c4878-138">アイテムが共有されました。</span><span class="sxs-lookup"><span data-stu-id="c4878-138">An item was shared.</span></span>
| <span data-ttu-id="c4878-139">version</span><span class="sxs-lookup"><span data-stu-id="c4878-139">version</span></span>       | <span data-ttu-id="c4878-140">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="c4878-140">[versionAction][]</span></span> | <span data-ttu-id="c4878-141">アイテムのバージョンが更新されました。</span><span class="sxs-lookup"><span data-stu-id="c4878-141">An item was versioned.</span></span>

[commentAction]: commentaction.md
[createAction]: createaction.md
[deleteAction]: deleteaction.md
[editAction]: editaction.md
[mentionAction]: mentionaction.md
[moveAction]: moveaction.md
[renameAction]: renameaction.md
[restoreAction]: restoreaction.md
[shareAction]: shareaction.md
[versionAction]: versionaction.md

## <a name="json-representation"></a><span data-ttu-id="c4878-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c4878-152">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActionSet",
  "@type.aka": "oneDrive.action"
}-->

```json
{
  "comment": {"@odata.type": "microsoft.graph.commentAction"},
  "create": {"@odata.type": "microsoft.graph.createAction"},
  "delete": {"@odata.type": "microsoft.graph.deleteAction"},
  "edit": {"@odata.type": "microsoft.graph.editAction"},
  "mention": {"@odata.type": "microsoft.graph.mentionAction"},
  "move": {"@odata.type": "microsoft.graph.moveAction"},
  "rename": {"@odata.type": "microsoft.graph.renameAction"},
  "restore": {"@odata.type": "microsoft.graph.restoreAction"},
  "share": {"@odata.type": "microsoft.graph.shareAction"},
  "version": {"@odata.type": "microsoft.graph.versionAction"},
  
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The itemActionSet object provides information about the actions that took place as part of an activity on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/itemActionSet",
  "suppressions": []
}
-->