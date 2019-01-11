---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionSet
localization_priority: Normal
ms.openlocfilehash: 194530da1df449d5ba523e084b2e72cd91bbe13d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873095"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="073d2-102">ItemActionSet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="073d2-102">ItemActionSet resource type</span></span>

> <span data-ttu-id="073d2-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="073d2-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="073d2-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="073d2-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="073d2-105">**ItemActionSet** リソースは、アイテムに対する[アクティビティ][itemActivity]を発生させたアクションに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="073d2-105">The **ItemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="073d2-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="073d2-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="073d2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="073d2-107">Properties</span></span>

<span data-ttu-id="073d2-108">現在使用可能なアクションを次に示します。</span><span class="sxs-lookup"><span data-stu-id="073d2-108">Below are the actions that are available today.</span></span>
<span data-ttu-id="073d2-109">将来、新しいアクションがログに記録される可能性があるため、アプリが認識するアクションがなくても、アプリが **itemActionSet** の処理を受け入れることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="073d2-109">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActionSet** without any actions that your app understands.</span></span>

| <span data-ttu-id="073d2-110">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="073d2-110">Property name</span></span> | <span data-ttu-id="073d2-111">Type</span><span class="sxs-lookup"><span data-stu-id="073d2-111">Type</span></span>              | <span data-ttu-id="073d2-112">説明</span><span class="sxs-lookup"><span data-stu-id="073d2-112">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="073d2-113">comment</span><span class="sxs-lookup"><span data-stu-id="073d2-113">comment</span></span>       | <span data-ttu-id="073d2-114">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="073d2-114">[commentAction][]</span></span> | <span data-ttu-id="073d2-115">アイテムにコメントが追加されました。</span><span class="sxs-lookup"><span data-stu-id="073d2-115">A comment was added to the item.</span></span>
| <span data-ttu-id="073d2-116">create</span><span class="sxs-lookup"><span data-stu-id="073d2-116">create</span></span>        | <span data-ttu-id="073d2-117">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="073d2-117">[createAction][]</span></span>  | <span data-ttu-id="073d2-118">アイテムが作成されました。</span><span class="sxs-lookup"><span data-stu-id="073d2-118">An item was created.</span></span>
| <span data-ttu-id="073d2-119">delete</span><span class="sxs-lookup"><span data-stu-id="073d2-119">delete</span></span>        | <span data-ttu-id="073d2-120">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="073d2-120">[deleteAction][]</span></span>  | <span data-ttu-id="073d2-121">アイテムが削除されました。</span><span class="sxs-lookup"><span data-stu-id="073d2-121">An item was deleted.</span></span>
| <span data-ttu-id="073d2-122">edit</span><span class="sxs-lookup"><span data-stu-id="073d2-122">edit</span></span>          | <span data-ttu-id="073d2-123">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="073d2-123">[editAction][]</span></span>    | <span data-ttu-id="073d2-124">アイテムが編集されました。</span><span class="sxs-lookup"><span data-stu-id="073d2-124">An item was edited.</span></span>
| <span data-ttu-id="073d2-125">mention</span><span class="sxs-lookup"><span data-stu-id="073d2-125">mention</span></span>       | <span data-ttu-id="073d2-126">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="073d2-126">[mentionAction][]</span></span> | <span data-ttu-id="073d2-127">アイテムでユーザーがメンションされました。</span><span class="sxs-lookup"><span data-stu-id="073d2-127">A user was mentioned in the item.</span></span>
| <span data-ttu-id="073d2-128">move</span><span class="sxs-lookup"><span data-stu-id="073d2-128">move</span></span>          | <span data-ttu-id="073d2-129">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="073d2-129">[moveAction][]</span></span>    | <span data-ttu-id="073d2-130">アイテムが移動されました。</span><span class="sxs-lookup"><span data-stu-id="073d2-130">An item was moved.</span></span>
| <span data-ttu-id="073d2-131">rename</span><span class="sxs-lookup"><span data-stu-id="073d2-131">rename</span></span>        | <span data-ttu-id="073d2-132">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="073d2-132">[renameAction][]</span></span>  | <span data-ttu-id="073d2-133">アイテムの名前が変更されました。</span><span class="sxs-lookup"><span data-stu-id="073d2-133">An item was renamed.</span></span>
| <span data-ttu-id="073d2-134">restore</span><span class="sxs-lookup"><span data-stu-id="073d2-134">restore</span></span>       | <span data-ttu-id="073d2-135">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="073d2-135">[restoreAction][]</span></span> | <span data-ttu-id="073d2-136">アイテムが復元されました。</span><span class="sxs-lookup"><span data-stu-id="073d2-136">An item was restored.</span></span>
| <span data-ttu-id="073d2-137">share</span><span class="sxs-lookup"><span data-stu-id="073d2-137">share</span></span>         | <span data-ttu-id="073d2-138">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="073d2-138">[shareAction][]</span></span>   | <span data-ttu-id="073d2-139">アイテムが共有されました。</span><span class="sxs-lookup"><span data-stu-id="073d2-139">An item was shared.</span></span>
| <span data-ttu-id="073d2-140">version</span><span class="sxs-lookup"><span data-stu-id="073d2-140">version</span></span>       | <span data-ttu-id="073d2-141">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="073d2-141">[versionAction][]</span></span> | <span data-ttu-id="073d2-142">アイテムのバージョンが更新されました。</span><span class="sxs-lookup"><span data-stu-id="073d2-142">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="073d2-153">備考</span><span class="sxs-lookup"><span data-stu-id="073d2-153">Remarks</span></span>

<span data-ttu-id="073d2-154">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="073d2-154">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about the actions that took place as part of an activity on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet"
} -->
