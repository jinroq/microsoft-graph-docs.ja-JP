---
title: outlooktaskfolder リソースの種類
description: 'Outlook のタスク (outlooktask オブジェクトのコレクション) が格納されているフォルダー。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d1299dda44cd698d0f6a1641f53557d2a7c8f342
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345577"
---
# <a name="outlooktaskfolder-resource-type"></a><span data-ttu-id="860cd-103">outlooktaskfolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="860cd-103">outlookTaskFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="860cd-104">Outlook のタスク ( [outlooktask](outlooktask.md)オブジェクトのコレクション) が格納されているフォルダー。</span><span class="sxs-lookup"><span data-stu-id="860cd-104">A folder that contains Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="860cd-105">Outlook では、既定のタスク グループ `My Tasks` には、ユーザーのメールボックス用の既定のタスク フォルダー `Tasks` が含まれています。</span><span class="sxs-lookup"><span data-stu-id="860cd-105">In Outlook, the default task group, `My Tasks`, contains a default task folder, `Tasks`, for the user's mailbox.</span></span> <span data-ttu-id="860cd-106">これらの既定のタスク グループとフォルダーの名前を変更したり削除したりすることはできませんが、タスク グループとタスク フォルダーを作成することはできます。</span><span class="sxs-lookup"><span data-stu-id="860cd-106">You cannot rename or delete these default task group and folder, but you can create additional task groups and task folders.</span></span>


## <a name="methods"></a><span data-ttu-id="860cd-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="860cd-107">Methods</span></span>

| <span data-ttu-id="860cd-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="860cd-108">Method</span></span>           | <span data-ttu-id="860cd-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="860cd-109">Return Type</span></span>    |<span data-ttu-id="860cd-110">説明</span><span class="sxs-lookup"><span data-stu-id="860cd-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="860cd-111">outlooktaskfolder の取得</span><span class="sxs-lookup"><span data-stu-id="860cd-111">Get outlookTaskFolder</span></span>](../api/outlooktaskfolder-get.md) | [<span data-ttu-id="860cd-112">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="860cd-112">outlookTaskFolder</span></span>](outlooktaskfolder.md) |<span data-ttu-id="860cd-113">指定された Outlook タスクフォルダーのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="860cd-113">Get the properties and relationships of the specified Outlook task folder.</span></span>|
|[<span data-ttu-id="860cd-114">outlooktask の作成</span><span class="sxs-lookup"><span data-stu-id="860cd-114">Create outlookTask</span></span>](../api/outlooktaskfolder-post-tasks.md) |[<span data-ttu-id="860cd-115">outlookTask</span><span class="sxs-lookup"><span data-stu-id="860cd-115">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="860cd-116">指定したタスクフォルダーに Outlook のタスクを作成します。</span><span class="sxs-lookup"><span data-stu-id="860cd-116">Create an Outlook task in the specified task folder.</span></span>|
|[<span data-ttu-id="860cd-117">タスクを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="860cd-117">List tasks</span></span>](../api/outlooktaskfolder-list-tasks.md) |<span data-ttu-id="860cd-118">[outlookTask](outlooktask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="860cd-118">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="860cd-119">指定したフォルダー内のすべての Outlook タスクを取得します。</span><span class="sxs-lookup"><span data-stu-id="860cd-119">Get all the Outlook tasks in the specified folder.</span></span>|
|[<span data-ttu-id="860cd-120">Update</span><span class="sxs-lookup"><span data-stu-id="860cd-120">Update</span></span>](../api/outlooktaskfolder-update.md) | [<span data-ttu-id="860cd-121">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="860cd-121">outlookTaskFolder</span></span>](outlooktaskfolder.md)   |<span data-ttu-id="860cd-122">Outlook タスクフォルダーの書き込み可能なプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="860cd-122">Update the writable properties of an Outlook task folder.</span></span> |
|[<span data-ttu-id="860cd-123">Delete</span><span class="sxs-lookup"><span data-stu-id="860cd-123">Delete</span></span>](../api/outlooktaskfolder-delete.md) | <span data-ttu-id="860cd-124">なし</span><span class="sxs-lookup"><span data-stu-id="860cd-124">None</span></span> |<span data-ttu-id="860cd-125">指定された Outlook タスクフォルダーを削除します。</span><span class="sxs-lookup"><span data-stu-id="860cd-125">Delete the specified Outlook task folder.</span></span>|
|<span data-ttu-id="860cd-126">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="860cd-126">**Extended properties**</span></span>| | |
|[<span data-ttu-id="860cd-127">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="860cd-127">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="860cd-128">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="860cd-128">outlookTaskFolder</span></span>](outlooktaskfolder.md)  |<span data-ttu-id="860cd-129">新規または既存の Outlook タスクフォルダーに、1つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="860cd-129">Create one or more single-value extended properties in a new or existing Outlook task folder.</span></span>   |
|[<span data-ttu-id="860cd-130">単一値の拡張プロパティを持つタスクフォルダーを取得する</span><span class="sxs-lookup"><span data-stu-id="860cd-130">Get task folder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="860cd-131">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="860cd-131">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="860cd-132">または`$expand` `$filter`を使用して、単一値の拡張プロパティを含む Outlook タスクフォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="860cd-132">Get Outlook task folders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="860cd-133">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="860cd-133">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="860cd-134">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="860cd-134">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="860cd-135">新規または既存の Outlook タスクフォルダーに、1つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="860cd-135">Create one or more multi-value extended properties in a new or existing Outlook task folder.</span></span>  |
|[<span data-ttu-id="860cd-136">複数値の拡張プロパティを持つタスクフォルダーを取得する</span><span class="sxs-lookup"><span data-stu-id="860cd-136">Get task folder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="860cd-137">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="860cd-137">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="860cd-138">を使用`$expand`して、複数値の拡張プロパティを含む Outlook のタスクフォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="860cd-138">Get an Outlook task folder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="860cd-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="860cd-139">Properties</span></span>
| <span data-ttu-id="860cd-140">プロパティ</span><span class="sxs-lookup"><span data-stu-id="860cd-140">Property</span></span>     | <span data-ttu-id="860cd-141">型</span><span class="sxs-lookup"><span data-stu-id="860cd-141">Type</span></span>   |<span data-ttu-id="860cd-142">説明</span><span class="sxs-lookup"><span data-stu-id="860cd-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="860cd-143">changeKey</span><span class="sxs-lookup"><span data-stu-id="860cd-143">changeKey</span></span>|<span data-ttu-id="860cd-144">String</span><span class="sxs-lookup"><span data-stu-id="860cd-144">String</span></span>|<span data-ttu-id="860cd-145">タスク フォルダーのバージョン。</span><span class="sxs-lookup"><span data-stu-id="860cd-145">The version of the task folder.</span></span>|
|<span data-ttu-id="860cd-146">id</span><span class="sxs-lookup"><span data-stu-id="860cd-146">id</span></span>|<span data-ttu-id="860cd-147">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="860cd-147">String</span></span>|<span data-ttu-id="860cd-148">ユーザーのメールボックス内で一意のタスクフォルダーの識別子。</span><span class="sxs-lookup"><span data-stu-id="860cd-148">The identifier of the task folder, unique in the user's mailbox.</span></span> <span data-ttu-id="860cd-149">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="860cd-149">Read-only.</span></span>|
|<span data-ttu-id="860cd-150">isdefaultfolder</span><span class="sxs-lookup"><span data-stu-id="860cd-150">isDefaultFolder</span></span>|<span data-ttu-id="860cd-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="860cd-151">Boolean</span></span>|<span data-ttu-id="860cd-152">フォルダーが既定のタスク フォルダーである場合は true。</span><span class="sxs-lookup"><span data-stu-id="860cd-152">True if the folder is the default task folder.</span></span>|
|<span data-ttu-id="860cd-153">name</span><span class="sxs-lookup"><span data-stu-id="860cd-153">name</span></span>|<span data-ttu-id="860cd-154">String</span><span class="sxs-lookup"><span data-stu-id="860cd-154">String</span></span>|<span data-ttu-id="860cd-155">タスク フォルダーの名前。</span><span class="sxs-lookup"><span data-stu-id="860cd-155">The name of the task folder.</span></span>|
|<span data-ttu-id="860cd-156">parentgroupkey</span><span class="sxs-lookup"><span data-stu-id="860cd-156">parentGroupKey</span></span>|<span data-ttu-id="860cd-157">Guid</span><span class="sxs-lookup"><span data-stu-id="860cd-157">Guid</span></span>|<span data-ttu-id="860cd-158">タスク フォルダーの親グループの一意の GUID 識別子。</span><span class="sxs-lookup"><span data-stu-id="860cd-158">The unique GUID identifier for the task folder's parent group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="860cd-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="860cd-159">Relationships</span></span>
| <span data-ttu-id="860cd-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="860cd-160">Relationship</span></span> | <span data-ttu-id="860cd-161">型</span><span class="sxs-lookup"><span data-stu-id="860cd-161">Type</span></span>   |<span data-ttu-id="860cd-162">説明</span><span class="sxs-lookup"><span data-stu-id="860cd-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="860cd-163">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="860cd-163">multiValueExtendedProperties</span></span>|<span data-ttu-id="860cd-164">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="860cd-164">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="860cd-165">タスクフォルダーに対して定義されている複数値の拡張プロパティのコレクション。</span><span class="sxs-lookup"><span data-stu-id="860cd-165">The collection of multi-value extended properties defined for the task folder.</span></span> <span data-ttu-id="860cd-166">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="860cd-166">Read-only.</span></span> <span data-ttu-id="860cd-167">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="860cd-167">Nullable.</span></span>|
|<span data-ttu-id="860cd-168">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="860cd-168">singleValueExtendedProperties</span></span>|<span data-ttu-id="860cd-169">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="860cd-169">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="860cd-170">タスクフォルダーに対して定義されている単一値の拡張プロパティのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="860cd-170">The collection of single-value extended properties defined for the task folder.</span></span> <span data-ttu-id="860cd-171">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="860cd-171">Read-only.</span></span> <span data-ttu-id="860cd-172">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="860cd-172">Nullable.</span></span>|
|<span data-ttu-id="860cd-173">tasks</span><span class="sxs-lookup"><span data-stu-id="860cd-173">tasks</span></span>|<span data-ttu-id="860cd-174">[outlookTask](outlooktask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="860cd-174">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="860cd-175">対象タスク フォルダー内のタスク。</span><span class="sxs-lookup"><span data-stu-id="860cd-175">The tasks in this task folder.</span></span> <span data-ttu-id="860cd-176">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="860cd-176">Read-only.</span></span> <span data-ttu-id="860cd-177">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="860cd-177">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="860cd-178">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="860cd-178">JSON representation</span></span>
<span data-ttu-id="860cd-179">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="860cd-179">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "multiValueExtendedProperties",
    "singleValueExtendedProperties",
    "tasks"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookTaskFolder"
}-->

```json
{
  "changeKey": "String",
  "id": "String (identifier)",
  "isDefaultFolder": true,
  "name": "String",
  "parentGroupKey": "Guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookTaskFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
