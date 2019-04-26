---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionSet
localization_priority: Normal
ms.openlocfilehash: b88f7514f7871e3c3850da91e4cd90b32f3a69c4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345410"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="726b4-102">ItemActionSet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="726b4-102">ItemActionSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="726b4-103">**ItemActionSet** リソースは、アイテムに対する[アクティビティ][itemActivity]を発生させたアクションに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="726b4-103">The **ItemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="726b4-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="726b4-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="726b4-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="726b4-105">Properties</span></span>

<span data-ttu-id="726b4-106">現在使用可能なアクションを次に示します。</span><span class="sxs-lookup"><span data-stu-id="726b4-106">Below are the actions that are available today.</span></span>
<span data-ttu-id="726b4-107">将来、新しいアクションがログに記録される可能性があるため、アプリが認識するアクションがなくても、アプリが **itemActionSet** の処理を受け入れることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="726b4-107">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActionSet** without any actions that your app understands.</span></span>

| <span data-ttu-id="726b4-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="726b4-108">Property name</span></span> | <span data-ttu-id="726b4-109">種類</span><span class="sxs-lookup"><span data-stu-id="726b4-109">Type</span></span>              | <span data-ttu-id="726b4-110">説明</span><span class="sxs-lookup"><span data-stu-id="726b4-110">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="726b4-111">comment</span><span class="sxs-lookup"><span data-stu-id="726b4-111">comment</span></span>       | <span data-ttu-id="726b4-112">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="726b4-112">[commentAction][]</span></span> | <span data-ttu-id="726b4-113">アイテムにコメントが追加されました。</span><span class="sxs-lookup"><span data-stu-id="726b4-113">A comment was added to the item.</span></span>
| <span data-ttu-id="726b4-114">create</span><span class="sxs-lookup"><span data-stu-id="726b4-114">create</span></span>        | <span data-ttu-id="726b4-115">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="726b4-115">[createAction][]</span></span>  | <span data-ttu-id="726b4-116">アイテムが作成されました。</span><span class="sxs-lookup"><span data-stu-id="726b4-116">An item was created.</span></span>
| <span data-ttu-id="726b4-117">delete</span><span class="sxs-lookup"><span data-stu-id="726b4-117">delete</span></span>        | <span data-ttu-id="726b4-118">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="726b4-118">[deleteAction][]</span></span>  | <span data-ttu-id="726b4-119">アイテムが削除されました。</span><span class="sxs-lookup"><span data-stu-id="726b4-119">An item was deleted.</span></span>
| <span data-ttu-id="726b4-120">edit</span><span class="sxs-lookup"><span data-stu-id="726b4-120">edit</span></span>          | <span data-ttu-id="726b4-121">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="726b4-121">[editAction][]</span></span>    | <span data-ttu-id="726b4-122">アイテムが編集されました。</span><span class="sxs-lookup"><span data-stu-id="726b4-122">An item was edited.</span></span>
| <span data-ttu-id="726b4-123">mention</span><span class="sxs-lookup"><span data-stu-id="726b4-123">mention</span></span>       | <span data-ttu-id="726b4-124">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="726b4-124">[mentionAction][]</span></span> | <span data-ttu-id="726b4-125">アイテムでユーザーがメンションされました。</span><span class="sxs-lookup"><span data-stu-id="726b4-125">A user was mentioned in the item.</span></span>
| <span data-ttu-id="726b4-126">move</span><span class="sxs-lookup"><span data-stu-id="726b4-126">move</span></span>          | <span data-ttu-id="726b4-127">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="726b4-127">[moveAction][]</span></span>    | <span data-ttu-id="726b4-128">アイテムが移動されました。</span><span class="sxs-lookup"><span data-stu-id="726b4-128">An item was moved.</span></span>
| <span data-ttu-id="726b4-129">rename</span><span class="sxs-lookup"><span data-stu-id="726b4-129">rename</span></span>        | <span data-ttu-id="726b4-130">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="726b4-130">[renameAction][]</span></span>  | <span data-ttu-id="726b4-131">アイテムの名前が変更されました。</span><span class="sxs-lookup"><span data-stu-id="726b4-131">An item was renamed.</span></span>
| <span data-ttu-id="726b4-132">restore</span><span class="sxs-lookup"><span data-stu-id="726b4-132">restore</span></span>       | <span data-ttu-id="726b4-133">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="726b4-133">[restoreAction][]</span></span> | <span data-ttu-id="726b4-134">アイテムが復元されました。</span><span class="sxs-lookup"><span data-stu-id="726b4-134">An item was restored.</span></span>
| <span data-ttu-id="726b4-135">share</span><span class="sxs-lookup"><span data-stu-id="726b4-135">share</span></span>         | <span data-ttu-id="726b4-136">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="726b4-136">[shareAction][]</span></span>   | <span data-ttu-id="726b4-137">アイテムが共有されました。</span><span class="sxs-lookup"><span data-stu-id="726b4-137">An item was shared.</span></span>
| <span data-ttu-id="726b4-138">version</span><span class="sxs-lookup"><span data-stu-id="726b4-138">version</span></span>       | <span data-ttu-id="726b4-139">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="726b4-139">[versionAction][]</span></span> | <span data-ttu-id="726b4-140">アイテムのバージョンが更新されました。</span><span class="sxs-lookup"><span data-stu-id="726b4-140">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="726b4-151">備考</span><span class="sxs-lookup"><span data-stu-id="726b4-151">Remarks</span></span>

<span data-ttu-id="726b4-152">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="726b4-152">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about the actions that took place as part of an activity on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet",
  "suppressions": []
}
-->
