---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: itemActivity
localization_priority: Normal
ms.openlocfilehash: 5e2be549c3e3e9e799449679b605577ecd782a94
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517296"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="55d92-102">ItemActivity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="55d92-102">ItemActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55d92-103">**ItemActivity** リソースは、アイテムまたはコンテナー内で発生したアクティビティについての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="55d92-103">The **ItemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="55d92-104">現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="55d92-104">Currently only available on SharePoint and OneDrive for Business.</span></span>

## <a name="json-representation"></a><span data-ttu-id="55d92-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="55d92-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="55d92-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55d92-106">Properties</span></span>

| <span data-ttu-id="55d92-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55d92-107">Property</span></span> | <span data-ttu-id="55d92-108">型</span><span class="sxs-lookup"><span data-stu-id="55d92-108">Type</span></span>                    | <span data-ttu-id="55d92-109">説明</span><span class="sxs-lookup"><span data-stu-id="55d92-109">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="55d92-110">id</span><span class="sxs-lookup"><span data-stu-id="55d92-110">id</span></span>       | <span data-ttu-id="55d92-111">string</span><span class="sxs-lookup"><span data-stu-id="55d92-111">string</span></span>                  | <span data-ttu-id="55d92-112">アクティビティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="55d92-112">The unique identifier of the activity.</span></span> <span data-ttu-id="55d92-113">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="55d92-113">Read-only.</span></span>
| <span data-ttu-id="55d92-114">Access</span><span class="sxs-lookup"><span data-stu-id="55d92-114">access</span></span>   | <span data-ttu-id="55d92-115">[accessAction][]</span><span class="sxs-lookup"><span data-stu-id="55d92-115">[accessAction][]</span></span>        | <span data-ttu-id="55d92-116">アイテムにアクセスしました。</span><span class="sxs-lookup"><span data-stu-id="55d92-116">An item was accessed.</span></span>
| <span data-ttu-id="55d92-117">action</span><span class="sxs-lookup"><span data-stu-id="55d92-117">action</span></span>   | <span data-ttu-id="55d92-118">[itemActionSet][]</span><span class="sxs-lookup"><span data-stu-id="55d92-118">[itemActionSet][]</span></span>       | <span data-ttu-id="55d92-119">発生したアクションについての詳細。</span><span class="sxs-lookup"><span data-stu-id="55d92-119">Details about the action that took place.</span></span> <span data-ttu-id="55d92-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="55d92-120">Read-only.</span></span>
| <span data-ttu-id="55d92-121">actor</span><span class="sxs-lookup"><span data-stu-id="55d92-121">actor</span></span>    | <span data-ttu-id="55d92-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="55d92-122">[identitySet][]</span></span>         | <span data-ttu-id="55d92-123">アクションを実行したユーザーの識別情報。</span><span class="sxs-lookup"><span data-stu-id="55d92-123">Identity of who performed the action.</span></span> <span data-ttu-id="55d92-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="55d92-124">Read-only.</span></span>
| <span data-ttu-id="55d92-125">location</span><span class="sxs-lookup"><span data-stu-id="55d92-125">location</span></span> | <span data-ttu-id="55d92-126">[location][]</span><span class="sxs-lookup"><span data-stu-id="55d92-126">[location][]</span></span>            | <span data-ttu-id="55d92-127">物理的な場所が、アクションが実行されました。</span><span class="sxs-lookup"><span data-stu-id="55d92-127">Physical location where the action was performed.</span></span> <span data-ttu-id="55d92-128">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="55d92-128">Read-only.</span></span>
| <span data-ttu-id="55d92-129">times</span><span class="sxs-lookup"><span data-stu-id="55d92-129">times</span></span>    | <span data-ttu-id="55d92-130">[itemActivityTimeSet][]</span><span class="sxs-lookup"><span data-stu-id="55d92-130">[itemActivityTimeSet][]</span></span> | <span data-ttu-id="55d92-131">アクティビティがいつ発生したかについての詳細。</span><span class="sxs-lookup"><span data-stu-id="55d92-131">Details about when the activity took place.</span></span> <span data-ttu-id="55d92-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="55d92-132">Read-only.</span></span>

[identitySet]: identityset.md
[itemActionSet]: itemactionset.md
[itemActivityTimeSet]: itemactivitytimeset.md

## <a name="relationships"></a><span data-ttu-id="55d92-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="55d92-136">Relationships</span></span>

| <span data-ttu-id="55d92-137">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="55d92-137">Relationship name</span></span> | <span data-ttu-id="55d92-138">型</span><span class="sxs-lookup"><span data-stu-id="55d92-138">Type</span></span>          | <span data-ttu-id="55d92-139">説明</span><span class="sxs-lookup"><span data-stu-id="55d92-139">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="55d92-140">driveItem</span><span class="sxs-lookup"><span data-stu-id="55d92-140">driveItem</span></span>         | <span data-ttu-id="55d92-141">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="55d92-141">[driveItem][]</span></span> | <span data-ttu-id="55d92-142">このアクティビティのターゲットとなった **driveItem** を表します。</span><span class="sxs-lookup"><span data-stu-id="55d92-142">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="55d92-143">listItem</span><span class="sxs-lookup"><span data-stu-id="55d92-143">listItem</span></span>          | <span data-ttu-id="55d92-144">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="55d92-144">[listItem][]</span></span>  | <span data-ttu-id="55d92-145">このアクティビティのターゲットとなった **listItem** を表します。</span><span class="sxs-lookup"><span data-stu-id="55d92-145">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="actions"></a><span data-ttu-id="55d92-148">アクション</span><span class="sxs-lookup"><span data-stu-id="55d92-148">Actions</span></span>

<span data-ttu-id="55d92-149">アクティビティ内で発生したアクションについては、**action** プロパティで詳しく記述されます。</span><span class="sxs-lookup"><span data-stu-id="55d92-149">The actions that took place within an activity are detailed in the **action** property.</span></span>
<span data-ttu-id="55d92-150">現在使用可能なアクションを次に示します。</span><span class="sxs-lookup"><span data-stu-id="55d92-150">Below are the actions that are available today.</span></span>
<span data-ttu-id="55d92-151">将来、新しいアクションがログに記録される可能性があるため、アプリが認識するアクションがなくても、アプリが **itemActivity** の処理を受け入れることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="55d92-151">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActivity** without any actions that your app understands.</span></span>

| <span data-ttu-id="55d92-152">アクション名</span><span class="sxs-lookup"><span data-stu-id="55d92-152">Action name</span></span> | <span data-ttu-id="55d92-153">種類</span><span class="sxs-lookup"><span data-stu-id="55d92-153">Type</span></span>              | <span data-ttu-id="55d92-154">説明</span><span class="sxs-lookup"><span data-stu-id="55d92-154">Description</span></span>
|:------------|:------------------|:-------------------------------------------
| <span data-ttu-id="55d92-155">comment</span><span class="sxs-lookup"><span data-stu-id="55d92-155">comment</span></span>     | <span data-ttu-id="55d92-156">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="55d92-156">[commentAction][]</span></span> | <span data-ttu-id="55d92-157">アイテムにコメントが追加されました。</span><span class="sxs-lookup"><span data-stu-id="55d92-157">A comment was added to the item.</span></span>
| <span data-ttu-id="55d92-158">create</span><span class="sxs-lookup"><span data-stu-id="55d92-158">create</span></span>      | <span data-ttu-id="55d92-159">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="55d92-159">[createAction][]</span></span>  | <span data-ttu-id="55d92-160">アイテムが作成されました。</span><span class="sxs-lookup"><span data-stu-id="55d92-160">An item was created.</span></span>
| <span data-ttu-id="55d92-161">delete</span><span class="sxs-lookup"><span data-stu-id="55d92-161">delete</span></span>      | <span data-ttu-id="55d92-162">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="55d92-162">[deleteAction][]</span></span>  | <span data-ttu-id="55d92-163">アイテムが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55d92-163">An item was deleted.</span></span>
| <span data-ttu-id="55d92-164">edit</span><span class="sxs-lookup"><span data-stu-id="55d92-164">edit</span></span>        | <span data-ttu-id="55d92-165">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="55d92-165">[editAction][]</span></span>    | <span data-ttu-id="55d92-166">アイテムが編集されました。</span><span class="sxs-lookup"><span data-stu-id="55d92-166">An item was edited.</span></span>
| <span data-ttu-id="55d92-167">mention</span><span class="sxs-lookup"><span data-stu-id="55d92-167">mention</span></span>     | <span data-ttu-id="55d92-168">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="55d92-168">[mentionAction][]</span></span> | <span data-ttu-id="55d92-169">アイテムでユーザーがメンションされました。</span><span class="sxs-lookup"><span data-stu-id="55d92-169">A user was mentioned in the item.</span></span>
| <span data-ttu-id="55d92-170">move</span><span class="sxs-lookup"><span data-stu-id="55d92-170">move</span></span>        | <span data-ttu-id="55d92-171">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="55d92-171">[moveAction][]</span></span>    | <span data-ttu-id="55d92-172">アイテムが移動されました。</span><span class="sxs-lookup"><span data-stu-id="55d92-172">An item was moved.</span></span>
| <span data-ttu-id="55d92-173">rename</span><span class="sxs-lookup"><span data-stu-id="55d92-173">rename</span></span>      | <span data-ttu-id="55d92-174">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="55d92-174">[renameAction][]</span></span>  | <span data-ttu-id="55d92-175">アイテムの名前が変更されました。</span><span class="sxs-lookup"><span data-stu-id="55d92-175">An item was renamed.</span></span>
| <span data-ttu-id="55d92-176">restore</span><span class="sxs-lookup"><span data-stu-id="55d92-176">restore</span></span>     | <span data-ttu-id="55d92-177">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="55d92-177">[restoreAction][]</span></span> | <span data-ttu-id="55d92-178">アイテムが復元されました。</span><span class="sxs-lookup"><span data-stu-id="55d92-178">An item was restored.</span></span>
| <span data-ttu-id="55d92-179">share</span><span class="sxs-lookup"><span data-stu-id="55d92-179">share</span></span>       | <span data-ttu-id="55d92-180">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="55d92-180">[shareAction][]</span></span>   | <span data-ttu-id="55d92-181">アイテムが共有されました。</span><span class="sxs-lookup"><span data-stu-id="55d92-181">An item was shared.</span></span>
| <span data-ttu-id="55d92-182">version</span><span class="sxs-lookup"><span data-stu-id="55d92-182">version</span></span>     | <span data-ttu-id="55d92-183">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="55d92-183">[versionAction][]</span></span> | <span data-ttu-id="55d92-184">アイテムのバージョンが更新されました。</span><span class="sxs-lookup"><span data-stu-id="55d92-184">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="55d92-197">備考</span><span class="sxs-lookup"><span data-stu-id="55d92-197">Remarks</span></span>

<span data-ttu-id="55d92-198">現在、**ItemActivity** は SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="55d92-198">**ItemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActivity",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemactivity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
