---
author: daspek
description: ItemActionSet リソースは、アイテムに対する [activity] [itemActivity] を構成したアクションに関する情報を提供します。
ms.date: 09/14/2017
title: ItemActionSet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8053942fe96011b018e46681d69d308f65aa5d5f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967148"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="293df-103">ItemActionSet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="293df-103">ItemActionSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="293df-104">**ItemActionSet** リソースは、アイテムに対する[アクティビティ][itemActivity]を発生させたアクションに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="293df-104">The **ItemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="293df-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="293df-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="293df-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="293df-106">Properties</span></span>

<span data-ttu-id="293df-107">現在使用可能なアクションを次に示します。</span><span class="sxs-lookup"><span data-stu-id="293df-107">Below are the actions that are available today.</span></span>
<span data-ttu-id="293df-108">将来、新しいアクションがログに記録される可能性があるため、アプリが認識するアクションがなくても、アプリが **itemActionSet** の処理を受け入れることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="293df-108">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActionSet** without any actions that your app understands.</span></span>

| <span data-ttu-id="293df-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="293df-109">Property name</span></span> | <span data-ttu-id="293df-110">種類</span><span class="sxs-lookup"><span data-stu-id="293df-110">Type</span></span>              | <span data-ttu-id="293df-111">説明</span><span class="sxs-lookup"><span data-stu-id="293df-111">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="293df-112">comment</span><span class="sxs-lookup"><span data-stu-id="293df-112">comment</span></span>       | <span data-ttu-id="293df-113">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="293df-113">[commentAction][]</span></span> | <span data-ttu-id="293df-114">アイテムにコメントが追加されました。</span><span class="sxs-lookup"><span data-stu-id="293df-114">A comment was added to the item.</span></span>
| <span data-ttu-id="293df-115">create</span><span class="sxs-lookup"><span data-stu-id="293df-115">create</span></span>        | <span data-ttu-id="293df-116">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="293df-116">[createAction][]</span></span>  | <span data-ttu-id="293df-117">アイテムが作成されました。</span><span class="sxs-lookup"><span data-stu-id="293df-117">An item was created.</span></span>
| <span data-ttu-id="293df-118">delete</span><span class="sxs-lookup"><span data-stu-id="293df-118">delete</span></span>        | <span data-ttu-id="293df-119">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="293df-119">[deleteAction][]</span></span>  | <span data-ttu-id="293df-120">アイテムが削除されました。</span><span class="sxs-lookup"><span data-stu-id="293df-120">An item was deleted.</span></span>
| <span data-ttu-id="293df-121">edit</span><span class="sxs-lookup"><span data-stu-id="293df-121">edit</span></span>          | <span data-ttu-id="293df-122">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="293df-122">[editAction][]</span></span>    | <span data-ttu-id="293df-123">アイテムが編集されました。</span><span class="sxs-lookup"><span data-stu-id="293df-123">An item was edited.</span></span>
| <span data-ttu-id="293df-124">mention</span><span class="sxs-lookup"><span data-stu-id="293df-124">mention</span></span>       | <span data-ttu-id="293df-125">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="293df-125">[mentionAction][]</span></span> | <span data-ttu-id="293df-126">アイテムでユーザーがメンションされました。</span><span class="sxs-lookup"><span data-stu-id="293df-126">A user was mentioned in the item.</span></span>
| <span data-ttu-id="293df-127">move</span><span class="sxs-lookup"><span data-stu-id="293df-127">move</span></span>          | <span data-ttu-id="293df-128">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="293df-128">[moveAction][]</span></span>    | <span data-ttu-id="293df-129">アイテムが移動されました。</span><span class="sxs-lookup"><span data-stu-id="293df-129">An item was moved.</span></span>
| <span data-ttu-id="293df-130">rename</span><span class="sxs-lookup"><span data-stu-id="293df-130">rename</span></span>        | <span data-ttu-id="293df-131">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="293df-131">[renameAction][]</span></span>  | <span data-ttu-id="293df-132">アイテムの名前が変更されました。</span><span class="sxs-lookup"><span data-stu-id="293df-132">An item was renamed.</span></span>
| <span data-ttu-id="293df-133">restore</span><span class="sxs-lookup"><span data-stu-id="293df-133">restore</span></span>       | <span data-ttu-id="293df-134">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="293df-134">[restoreAction][]</span></span> | <span data-ttu-id="293df-135">アイテムが復元されました。</span><span class="sxs-lookup"><span data-stu-id="293df-135">An item was restored.</span></span>
| <span data-ttu-id="293df-136">share</span><span class="sxs-lookup"><span data-stu-id="293df-136">share</span></span>         | <span data-ttu-id="293df-137">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="293df-137">[shareAction][]</span></span>   | <span data-ttu-id="293df-138">アイテムが共有されました。</span><span class="sxs-lookup"><span data-stu-id="293df-138">An item was shared.</span></span>
| <span data-ttu-id="293df-139">version</span><span class="sxs-lookup"><span data-stu-id="293df-139">version</span></span>       | <span data-ttu-id="293df-140">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="293df-140">[versionAction][]</span></span> | <span data-ttu-id="293df-141">アイテムのバージョンが更新されました。</span><span class="sxs-lookup"><span data-stu-id="293df-141">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="293df-152">備考</span><span class="sxs-lookup"><span data-stu-id="293df-152">Remarks</span></span>

<span data-ttu-id="293df-153">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="293df-153">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
