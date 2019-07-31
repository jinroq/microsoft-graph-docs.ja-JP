---
author: daspek
description: ItemActivity リソースは、アイテムまたはコンテナー内で発生したアクティビティについての情報を提供します。
ms.date: 09/14/2017
title: ItemActivity
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: ab96c3169a2d2dc37e6b94ab325866e93fa4d6c0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967101"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="dfc0d-103">ItemActivity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dfc0d-103">ItemActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfc0d-104">**ItemActivity** リソースは、アイテムまたはコンテナー内で発生したアクティビティについての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-104">The **ItemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="dfc0d-105">現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-105">Currently only available on SharePoint and OneDrive for Business.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dfc0d-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dfc0d-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="dfc0d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfc0d-107">Properties</span></span>

| <span data-ttu-id="dfc0d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfc0d-108">Property</span></span> | <span data-ttu-id="dfc0d-109">型</span><span class="sxs-lookup"><span data-stu-id="dfc0d-109">Type</span></span>                    | <span data-ttu-id="dfc0d-110">説明</span><span class="sxs-lookup"><span data-stu-id="dfc0d-110">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="dfc0d-111">id</span><span class="sxs-lookup"><span data-stu-id="dfc0d-111">id</span></span>       | <span data-ttu-id="dfc0d-112">string</span><span class="sxs-lookup"><span data-stu-id="dfc0d-112">string</span></span>                  | <span data-ttu-id="dfc0d-113">アクティビティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-113">The unique identifier of the activity.</span></span> <span data-ttu-id="dfc0d-114">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-114">Read-only.</span></span>
| <span data-ttu-id="dfc0d-115">接続</span><span class="sxs-lookup"><span data-stu-id="dfc0d-115">access</span></span>   | <span data-ttu-id="dfc0d-116">[accessAction][]</span><span class="sxs-lookup"><span data-stu-id="dfc0d-116">[accessAction][]</span></span>        | <span data-ttu-id="dfc0d-117">アイテムがアクセスされました。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-117">An item was accessed.</span></span>
| <span data-ttu-id="dfc0d-118">action</span><span class="sxs-lookup"><span data-stu-id="dfc0d-118">action</span></span>   | <span data-ttu-id="dfc0d-119">[itemActionSet][]</span><span class="sxs-lookup"><span data-stu-id="dfc0d-119">[itemActionSet][]</span></span>       | <span data-ttu-id="dfc0d-120">発生したアクションについての詳細。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-120">Details about the action that took place.</span></span> <span data-ttu-id="dfc0d-121">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-121">Read-only.</span></span>
| <span data-ttu-id="dfc0d-122">actor</span><span class="sxs-lookup"><span data-stu-id="dfc0d-122">actor</span></span>    | <span data-ttu-id="dfc0d-123">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="dfc0d-123">[identitySet][]</span></span>         | <span data-ttu-id="dfc0d-124">アクションを実行したユーザーの識別情報。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-124">Identity of who performed the action.</span></span> <span data-ttu-id="dfc0d-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-125">Read-only.</span></span>
| <span data-ttu-id="dfc0d-126">location</span><span class="sxs-lookup"><span data-stu-id="dfc0d-126">location</span></span> | <span data-ttu-id="dfc0d-127">[location][]</span><span class="sxs-lookup"><span data-stu-id="dfc0d-127">[location][]</span></span>            | <span data-ttu-id="dfc0d-128">アクションが実行された物理的な場所。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-128">Physical location where the action was performed.</span></span> <span data-ttu-id="dfc0d-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-129">Read-only.</span></span>
| <span data-ttu-id="dfc0d-130">times</span><span class="sxs-lookup"><span data-stu-id="dfc0d-130">times</span></span>    | <span data-ttu-id="dfc0d-131">[itemActivityTimeSet][]</span><span class="sxs-lookup"><span data-stu-id="dfc0d-131">[itemActivityTimeSet][]</span></span> | <span data-ttu-id="dfc0d-132">アクティビティがいつ発生したかについての詳細。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-132">Details about when the activity took place.</span></span> <span data-ttu-id="dfc0d-133">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-133">Read-only.</span></span>

[identitySet]: identityset.md
[itemActionSet]: itemactionset.md
[itemActivityTimeSet]: itemactivitytimeset.md

## <a name="relationships"></a><span data-ttu-id="dfc0d-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dfc0d-137">Relationships</span></span>

| <span data-ttu-id="dfc0d-138">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="dfc0d-138">Relationship name</span></span> | <span data-ttu-id="dfc0d-139">種類</span><span class="sxs-lookup"><span data-stu-id="dfc0d-139">Type</span></span>          | <span data-ttu-id="dfc0d-140">説明</span><span class="sxs-lookup"><span data-stu-id="dfc0d-140">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="dfc0d-141">driveItem</span><span class="sxs-lookup"><span data-stu-id="dfc0d-141">driveItem</span></span>         | <span data-ttu-id="dfc0d-142">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="dfc0d-142">[driveItem][]</span></span> | <span data-ttu-id="dfc0d-143">このアクティビティのターゲットとなった **driveItem** を表します。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-143">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="dfc0d-144">listItem</span><span class="sxs-lookup"><span data-stu-id="dfc0d-144">listItem</span></span>          | <span data-ttu-id="dfc0d-145">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="dfc0d-145">[listItem][]</span></span>  | <span data-ttu-id="dfc0d-146">このアクティビティのターゲットとなった **listItem** を表します。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-146">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="actions"></a><span data-ttu-id="dfc0d-149">アクション</span><span class="sxs-lookup"><span data-stu-id="dfc0d-149">Actions</span></span>

<span data-ttu-id="dfc0d-150">アクティビティ内で発生したアクションについては、**action** プロパティで詳しく記述されます。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-150">The actions that took place within an activity are detailed in the **action** property.</span></span>
<span data-ttu-id="dfc0d-151">現在使用可能なアクションを次に示します。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-151">Below are the actions that are available today.</span></span>
<span data-ttu-id="dfc0d-152">将来、新しいアクションがログに記録される可能性があるため、アプリが認識するアクションがなくても、アプリが **itemActivity** の処理を受け入れることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-152">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActivity** without any actions that your app understands.</span></span>

| <span data-ttu-id="dfc0d-153">アクション名</span><span class="sxs-lookup"><span data-stu-id="dfc0d-153">Action name</span></span> | <span data-ttu-id="dfc0d-154">型</span><span class="sxs-lookup"><span data-stu-id="dfc0d-154">Type</span></span>              | <span data-ttu-id="dfc0d-155">説明</span><span class="sxs-lookup"><span data-stu-id="dfc0d-155">Description</span></span>
|:------------|:------------------|:-------------------------------------------
| <span data-ttu-id="dfc0d-156">comment</span><span class="sxs-lookup"><span data-stu-id="dfc0d-156">comment</span></span>     | <span data-ttu-id="dfc0d-157">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="dfc0d-157">[commentAction][]</span></span> | <span data-ttu-id="dfc0d-158">アイテムにコメントが追加されました。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-158">A comment was added to the item.</span></span>
| <span data-ttu-id="dfc0d-159">create</span><span class="sxs-lookup"><span data-stu-id="dfc0d-159">create</span></span>      | <span data-ttu-id="dfc0d-160">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="dfc0d-160">[createAction][]</span></span>  | <span data-ttu-id="dfc0d-161">アイテムが作成されました。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-161">An item was created.</span></span>
| <span data-ttu-id="dfc0d-162">delete</span><span class="sxs-lookup"><span data-stu-id="dfc0d-162">delete</span></span>      | <span data-ttu-id="dfc0d-163">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="dfc0d-163">[deleteAction][]</span></span>  | <span data-ttu-id="dfc0d-164">アイテムが削除されました。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-164">An item was deleted.</span></span>
| <span data-ttu-id="dfc0d-165">edit</span><span class="sxs-lookup"><span data-stu-id="dfc0d-165">edit</span></span>        | <span data-ttu-id="dfc0d-166">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="dfc0d-166">[editAction][]</span></span>    | <span data-ttu-id="dfc0d-167">アイテムが編集されました。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-167">An item was edited.</span></span>
| <span data-ttu-id="dfc0d-168">mention</span><span class="sxs-lookup"><span data-stu-id="dfc0d-168">mention</span></span>     | <span data-ttu-id="dfc0d-169">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="dfc0d-169">[mentionAction][]</span></span> | <span data-ttu-id="dfc0d-170">アイテムでユーザーがメンションされました。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-170">A user was mentioned in the item.</span></span>
| <span data-ttu-id="dfc0d-171">move</span><span class="sxs-lookup"><span data-stu-id="dfc0d-171">move</span></span>        | <span data-ttu-id="dfc0d-172">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="dfc0d-172">[moveAction][]</span></span>    | <span data-ttu-id="dfc0d-173">アイテムが移動されました。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-173">An item was moved.</span></span>
| <span data-ttu-id="dfc0d-174">rename</span><span class="sxs-lookup"><span data-stu-id="dfc0d-174">rename</span></span>      | <span data-ttu-id="dfc0d-175">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="dfc0d-175">[renameAction][]</span></span>  | <span data-ttu-id="dfc0d-176">アイテムの名前が変更されました。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-176">An item was renamed.</span></span>
| <span data-ttu-id="dfc0d-177">restore</span><span class="sxs-lookup"><span data-stu-id="dfc0d-177">restore</span></span>     | <span data-ttu-id="dfc0d-178">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="dfc0d-178">[restoreAction][]</span></span> | <span data-ttu-id="dfc0d-179">アイテムが復元されました。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-179">An item was restored.</span></span>
| <span data-ttu-id="dfc0d-180">share</span><span class="sxs-lookup"><span data-stu-id="dfc0d-180">share</span></span>       | <span data-ttu-id="dfc0d-181">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="dfc0d-181">[shareAction][]</span></span>   | <span data-ttu-id="dfc0d-182">アイテムが共有されました。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-182">An item was shared.</span></span>
| <span data-ttu-id="dfc0d-183">version</span><span class="sxs-lookup"><span data-stu-id="dfc0d-183">version</span></span>     | <span data-ttu-id="dfc0d-184">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="dfc0d-184">[versionAction][]</span></span> | <span data-ttu-id="dfc0d-185">アイテムのバージョンが更新されました。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-185">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="dfc0d-198">備考</span><span class="sxs-lookup"><span data-stu-id="dfc0d-198">Remarks</span></span>

<span data-ttu-id="dfc0d-199">現在、**ItemActivity** は SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="dfc0d-199">**ItemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActivity",
  "suppressions": []
}
-->
