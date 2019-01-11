---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivity
localization_priority: Normal
ms.openlocfilehash: a29bdad0ae5e06d3d1b55f1fb7ceb630bec1b564
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819671"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="d9154-102">ItemActivity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d9154-102">ItemActivity resource type</span></span>

> <span data-ttu-id="d9154-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d9154-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9154-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9154-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d9154-105">**ItemActivity** リソースは、アイテムまたはコンテナー内で発生したアクティビティについての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="d9154-105">The **ItemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="d9154-106">現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="d9154-106">Currently only available on SharePoint and OneDrive for Business.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9154-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d9154-107">JSON representation</span></span>

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
  "action": {"@odata.type": "microsoft.graph.itemActionSet"},
  "actor": {"@odata.type": "microsoft.graph.identitySet"},
  "driveItem": {"@odata.type": "microsoft.graph.driveItem"},
  "listItem": {"@odata.type": "microsoft.graph.listItem"},
  "location": {"@odata.type": "microsoft.graph.location"},
  "times": {"@odata.type": "microsoft.graph.itemActivityTimeSet"}
}
```

## <a name="properties"></a><span data-ttu-id="d9154-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d9154-108">Properties</span></span>

| <span data-ttu-id="d9154-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d9154-109">Property</span></span> | <span data-ttu-id="d9154-110">種類</span><span class="sxs-lookup"><span data-stu-id="d9154-110">Type</span></span>                    | <span data-ttu-id="d9154-111">説明</span><span class="sxs-lookup"><span data-stu-id="d9154-111">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="d9154-112">ID</span><span class="sxs-lookup"><span data-stu-id="d9154-112">id</span></span>       | <span data-ttu-id="d9154-113">文字列</span><span class="sxs-lookup"><span data-stu-id="d9154-113">string</span></span>                  | <span data-ttu-id="d9154-114">アクティビティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="d9154-114">The unique identifier of the activity.</span></span> <span data-ttu-id="d9154-115">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d9154-115">Read-only.</span></span>
| <span data-ttu-id="d9154-116">アクセス</span><span class="sxs-lookup"><span data-stu-id="d9154-116">access</span></span>   | <span data-ttu-id="d9154-117">[accessAction][]</span><span class="sxs-lookup"><span data-stu-id="d9154-117">[accessAction][]</span></span>        | <span data-ttu-id="d9154-118">アイテムにアクセスしました。</span><span class="sxs-lookup"><span data-stu-id="d9154-118">An item was accessed.</span></span>
| <span data-ttu-id="d9154-119">action</span><span class="sxs-lookup"><span data-stu-id="d9154-119">action</span></span>   | <span data-ttu-id="d9154-120">[itemActionSet][]</span><span class="sxs-lookup"><span data-stu-id="d9154-120">[itemActionSet][]</span></span>       | <span data-ttu-id="d9154-121">発生したアクションについての詳細。</span><span class="sxs-lookup"><span data-stu-id="d9154-121">Details about the action that took place.</span></span> <span data-ttu-id="d9154-122">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d9154-122">Read-only.</span></span>
| <span data-ttu-id="d9154-123">actor</span><span class="sxs-lookup"><span data-stu-id="d9154-123">actor</span></span>    | <span data-ttu-id="d9154-124">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="d9154-124">[identitySet][]</span></span>         | <span data-ttu-id="d9154-125">アクションを実行したユーザーの識別情報。</span><span class="sxs-lookup"><span data-stu-id="d9154-125">Identity of who performed the action.</span></span> <span data-ttu-id="d9154-126">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d9154-126">Read-only.</span></span>
| <span data-ttu-id="d9154-127">location</span><span class="sxs-lookup"><span data-stu-id="d9154-127">location</span></span> | <span data-ttu-id="d9154-128">[location][]</span><span class="sxs-lookup"><span data-stu-id="d9154-128">[location][]</span></span>            | <span data-ttu-id="d9154-129">物理的な場所が、アクションが実行されました。</span><span class="sxs-lookup"><span data-stu-id="d9154-129">Physical location where the action was performed.</span></span> <span data-ttu-id="d9154-130">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d9154-130">Read-only.</span></span>
| <span data-ttu-id="d9154-131">times</span><span class="sxs-lookup"><span data-stu-id="d9154-131">times</span></span>    | <span data-ttu-id="d9154-132">[itemActivityTimeSet][]</span><span class="sxs-lookup"><span data-stu-id="d9154-132">[itemActivityTimeSet][]</span></span> | <span data-ttu-id="d9154-133">アクティビティがいつ発生したかについての詳細。</span><span class="sxs-lookup"><span data-stu-id="d9154-133">Details about when the activity took place.</span></span> <span data-ttu-id="d9154-134">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d9154-134">Read-only.</span></span>

[identitySet]: identityset.md
[itemActionSet]: itemactionset.md
[itemActivityTimeSet]: itemactivitytimeset.md

## <a name="relationships"></a><span data-ttu-id="d9154-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d9154-138">Relationships</span></span>

| <span data-ttu-id="d9154-139">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="d9154-139">Relationship name</span></span> | <span data-ttu-id="d9154-140">種類</span><span class="sxs-lookup"><span data-stu-id="d9154-140">Type</span></span>          | <span data-ttu-id="d9154-141">説明</span><span class="sxs-lookup"><span data-stu-id="d9154-141">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="d9154-142">driveItem</span><span class="sxs-lookup"><span data-stu-id="d9154-142">driveItem</span></span>         | <span data-ttu-id="d9154-143">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="d9154-143">[driveItem][]</span></span> | <span data-ttu-id="d9154-144">このアクティビティのターゲットとなった **driveItem** を表します。</span><span class="sxs-lookup"><span data-stu-id="d9154-144">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="d9154-145">listItem</span><span class="sxs-lookup"><span data-stu-id="d9154-145">listItem</span></span>          | <span data-ttu-id="d9154-146">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="d9154-146">[listItem][]</span></span>  | <span data-ttu-id="d9154-147">このアクティビティのターゲットとなった **listItem** を表します。</span><span class="sxs-lookup"><span data-stu-id="d9154-147">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="actions"></a><span data-ttu-id="d9154-150">アクション</span><span class="sxs-lookup"><span data-stu-id="d9154-150">Actions</span></span>

<span data-ttu-id="d9154-151">アクティビティ内で発生したアクションについては、**action** プロパティで詳しく記述されます。</span><span class="sxs-lookup"><span data-stu-id="d9154-151">The actions that took place within an activity are detailed in the **action** property.</span></span>
<span data-ttu-id="d9154-152">現在使用可能なアクションを次に示します。</span><span class="sxs-lookup"><span data-stu-id="d9154-152">Below are the actions that are available today.</span></span>
<span data-ttu-id="d9154-153">将来、新しいアクションがログに記録される可能性があるため、アプリが認識するアクションがなくても、アプリが **itemActivity** の処理を受け入れることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="d9154-153">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActivity** without any actions that your app understands.</span></span>

| <span data-ttu-id="d9154-154">アクション名</span><span class="sxs-lookup"><span data-stu-id="d9154-154">Action name</span></span> | <span data-ttu-id="d9154-155">種類</span><span class="sxs-lookup"><span data-stu-id="d9154-155">Type</span></span>              | <span data-ttu-id="d9154-156">説明</span><span class="sxs-lookup"><span data-stu-id="d9154-156">Description</span></span>
|:------------|:------------------|:-------------------------------------------
| <span data-ttu-id="d9154-157">comment</span><span class="sxs-lookup"><span data-stu-id="d9154-157">comment</span></span>     | <span data-ttu-id="d9154-158">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="d9154-158">[commentAction][]</span></span> | <span data-ttu-id="d9154-159">アイテムにコメントが追加されました。</span><span class="sxs-lookup"><span data-stu-id="d9154-159">A comment was added to the item.</span></span>
| <span data-ttu-id="d9154-160">create</span><span class="sxs-lookup"><span data-stu-id="d9154-160">create</span></span>      | <span data-ttu-id="d9154-161">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="d9154-161">[createAction][]</span></span>  | <span data-ttu-id="d9154-162">アイテムが作成されました。</span><span class="sxs-lookup"><span data-stu-id="d9154-162">An item was created.</span></span>
| <span data-ttu-id="d9154-163">delete</span><span class="sxs-lookup"><span data-stu-id="d9154-163">delete</span></span>      | <span data-ttu-id="d9154-164">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="d9154-164">[deleteAction][]</span></span>  | <span data-ttu-id="d9154-165">アイテムが削除されました。</span><span class="sxs-lookup"><span data-stu-id="d9154-165">An item was deleted.</span></span>
| <span data-ttu-id="d9154-166">edit</span><span class="sxs-lookup"><span data-stu-id="d9154-166">edit</span></span>        | <span data-ttu-id="d9154-167">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="d9154-167">[editAction][]</span></span>    | <span data-ttu-id="d9154-168">アイテムが編集されました。</span><span class="sxs-lookup"><span data-stu-id="d9154-168">An item was edited.</span></span>
| <span data-ttu-id="d9154-169">mention</span><span class="sxs-lookup"><span data-stu-id="d9154-169">mention</span></span>     | <span data-ttu-id="d9154-170">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="d9154-170">[mentionAction][]</span></span> | <span data-ttu-id="d9154-171">アイテムでユーザーがメンションされました。</span><span class="sxs-lookup"><span data-stu-id="d9154-171">A user was mentioned in the item.</span></span>
| <span data-ttu-id="d9154-172">move</span><span class="sxs-lookup"><span data-stu-id="d9154-172">move</span></span>        | <span data-ttu-id="d9154-173">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="d9154-173">[moveAction][]</span></span>    | <span data-ttu-id="d9154-174">アイテムが移動されました。</span><span class="sxs-lookup"><span data-stu-id="d9154-174">An item was moved.</span></span>
| <span data-ttu-id="d9154-175">rename</span><span class="sxs-lookup"><span data-stu-id="d9154-175">rename</span></span>      | <span data-ttu-id="d9154-176">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="d9154-176">[renameAction][]</span></span>  | <span data-ttu-id="d9154-177">アイテムの名前が変更されました。</span><span class="sxs-lookup"><span data-stu-id="d9154-177">An item was renamed.</span></span>
| <span data-ttu-id="d9154-178">restore</span><span class="sxs-lookup"><span data-stu-id="d9154-178">restore</span></span>     | <span data-ttu-id="d9154-179">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="d9154-179">[restoreAction][]</span></span> | <span data-ttu-id="d9154-180">アイテムが復元されました。</span><span class="sxs-lookup"><span data-stu-id="d9154-180">An item was restored.</span></span>
| <span data-ttu-id="d9154-181">share</span><span class="sxs-lookup"><span data-stu-id="d9154-181">share</span></span>       | <span data-ttu-id="d9154-182">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="d9154-182">[shareAction][]</span></span>   | <span data-ttu-id="d9154-183">アイテムが共有されました。</span><span class="sxs-lookup"><span data-stu-id="d9154-183">An item was shared.</span></span>
| <span data-ttu-id="d9154-184">version</span><span class="sxs-lookup"><span data-stu-id="d9154-184">version</span></span>     | <span data-ttu-id="d9154-185">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="d9154-185">[versionAction][]</span></span> | <span data-ttu-id="d9154-186">アイテムのバージョンが更新されました。</span><span class="sxs-lookup"><span data-stu-id="d9154-186">An item was versioned.</span></span>

[accessAction]: accessaction.md
[commentAction]: commentaction.md
[createAction]: createaction.md
[deleteAction]: deleteaction.md
[editAction]: editaction.md
[location]: location.md
[mentionAction]: mentionaction.md
[moveAction]: moveaction.md
[renameAction]: renameaction.md
[restoreAction]: restoreaction.md
[shareAction]: shareaction.md
[versionAction]: versionaction.md

## <a name="remarks"></a><span data-ttu-id="d9154-199">備考</span><span class="sxs-lookup"><span data-stu-id="d9154-199">Remarks</span></span>

<span data-ttu-id="d9154-200">現在、**ItemActivity** は SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="d9154-200">**ItemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActivity"
} -->
