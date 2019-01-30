---
title: outlookTaskFolder リソースの種類
description: 'Outlook のタスク (outlookTask オブジェクトのコレクション) を含むフォルダーです。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: eb61936b9ede67d35127db07c92ba8b7517fe623
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643924"
---
# <a name="outlooktaskfolder-resource-type"></a><span data-ttu-id="9aae7-103">outlookTaskFolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9aae7-103">outlookTaskFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9aae7-104">Outlook のタスク ( [outlookTask](outlooktask.md)オブジェクトのコレクション) を含むフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="9aae7-104">A folder that contains Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="9aae7-105">Outlook では、既定のタスク グループ `My Tasks` には、ユーザーのメールボックス用の既定のタスク フォルダー `Tasks` が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9aae7-105">In Outlook, the default task group, `My Tasks`, contains a default task folder, `Tasks`, for the user's mailbox.</span></span> <span data-ttu-id="9aae7-106">これらの既定のタスク グループとフォルダーの名前を変更したり削除したりすることはできませんが、タスク グループとタスク フォルダーを作成することはできます。</span><span class="sxs-lookup"><span data-stu-id="9aae7-106">You cannot rename or delete these default task group and folder, but you can create additional task groups and task folders.</span></span>


## <a name="methods"></a><span data-ttu-id="9aae7-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="9aae7-107">Methods</span></span>

| <span data-ttu-id="9aae7-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="9aae7-108">Method</span></span>           | <span data-ttu-id="9aae7-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9aae7-109">Return Type</span></span>    |<span data-ttu-id="9aae7-110">説明</span><span class="sxs-lookup"><span data-stu-id="9aae7-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9aae7-111">OutlookTaskFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="9aae7-111">Get outlookTaskFolder</span></span>](../api/outlooktaskfolder-get.md) | [<span data-ttu-id="9aae7-112">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="9aae7-112">outlookTaskFolder</span></span>](outlooktaskfolder.md) |<span data-ttu-id="9aae7-113">プロパティと指定した Outlook の仕事フォルダーの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="9aae7-113">Get the properties and relationships of the specified Outlook task folder.</span></span>|
|[<span data-ttu-id="9aae7-114">OutlookTask を作成します。</span><span class="sxs-lookup"><span data-stu-id="9aae7-114">Create outlookTask</span></span>](../api/outlooktaskfolder-post-tasks.md) |[<span data-ttu-id="9aae7-115">outlookTask</span><span class="sxs-lookup"><span data-stu-id="9aae7-115">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="9aae7-116">指定されたタスクのフォルダーに Outlook のタスクを作成します。</span><span class="sxs-lookup"><span data-stu-id="9aae7-116">Create an Outlook task in the specified task folder.</span></span>|
|[<span data-ttu-id="9aae7-117">List tasks</span><span class="sxs-lookup"><span data-stu-id="9aae7-117">List tasks</span></span>](../api/outlooktaskfolder-list-tasks.md) |<span data-ttu-id="9aae7-118">[outlookTask](outlooktask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9aae7-118">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="9aae7-119">指定したフォルダーに Outlook のすべてのタスクを取得します。</span><span class="sxs-lookup"><span data-stu-id="9aae7-119">Get all the Outlook tasks in the specified folder.</span></span>|
|[<span data-ttu-id="9aae7-120">更新する</span><span class="sxs-lookup"><span data-stu-id="9aae7-120">Update</span></span>](../api/outlooktaskfolder-update.md) | [<span data-ttu-id="9aae7-121">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="9aae7-121">outlookTaskFolder</span></span>](outlooktaskfolder.md)   |<span data-ttu-id="9aae7-122">Outlook の仕事フォルダーの書き込み可能なプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9aae7-122">Update the writable properties of an Outlook task folder.</span></span> |
|[<span data-ttu-id="9aae7-123">削除する</span><span class="sxs-lookup"><span data-stu-id="9aae7-123">Delete</span></span>](../api/outlooktaskfolder-delete.md) | <span data-ttu-id="9aae7-124">なし</span><span class="sxs-lookup"><span data-stu-id="9aae7-124">None</span></span> |<span data-ttu-id="9aae7-125">指定した Outlook の仕事フォルダーを削除します。</span><span class="sxs-lookup"><span data-stu-id="9aae7-125">Delete the specified Outlook task folder.</span></span>|
|<span data-ttu-id="9aae7-126">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="9aae7-126">**Extended properties**</span></span>| | |
|[<span data-ttu-id="9aae7-127">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="9aae7-127">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="9aae7-128">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="9aae7-128">outlookTaskFolder</span></span>](outlooktaskfolder.md)  |<span data-ttu-id="9aae7-129">新規または既存の Outlook タスク フォルダー内の 1 つまたは複数の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="9aae7-129">Create one or more single-value extended properties in a new or existing Outlook task folder.</span></span>   |
|[<span data-ttu-id="9aae7-130">拡張プロパティを単一値を持つタスク フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="9aae7-130">Get task folder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="9aae7-131">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="9aae7-131">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="9aae7-132">拡張プロパティを使用して単一の値が含まれている Outlook の仕事フォルダーを取得する`$expand`または`$filter`。</span><span class="sxs-lookup"><span data-stu-id="9aae7-132">Get Outlook task folders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="9aae7-133">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="9aae7-133">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="9aae7-134">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="9aae7-134">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="9aae7-135">新規または既存の Outlook タスク フォルダー内の 1 つまたは複数の値を複数の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="9aae7-135">Create one or more multi-value extended properties in a new or existing Outlook task folder.</span></span>  |
|[<span data-ttu-id="9aae7-136">拡張プロパティ値を複数の作業フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="9aae7-136">Get task folder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="9aae7-137">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="9aae7-137">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="9aae7-138">使用して複数の値の拡張プロパティを含む Outlook の仕事フォルダーを取得する`$expand`。</span><span class="sxs-lookup"><span data-stu-id="9aae7-138">Get an Outlook task folder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="9aae7-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9aae7-139">Properties</span></span>
| <span data-ttu-id="9aae7-140">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9aae7-140">Property</span></span>     | <span data-ttu-id="9aae7-141">型</span><span class="sxs-lookup"><span data-stu-id="9aae7-141">Type</span></span>   |<span data-ttu-id="9aae7-142">説明</span><span class="sxs-lookup"><span data-stu-id="9aae7-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9aae7-143">changeKey</span><span class="sxs-lookup"><span data-stu-id="9aae7-143">changeKey</span></span>|<span data-ttu-id="9aae7-144">String</span><span class="sxs-lookup"><span data-stu-id="9aae7-144">String</span></span>|<span data-ttu-id="9aae7-145">タスク フォルダーのバージョン。</span><span class="sxs-lookup"><span data-stu-id="9aae7-145">The version of the task folder.</span></span>|
|<span data-ttu-id="9aae7-146">id</span><span class="sxs-lookup"><span data-stu-id="9aae7-146">id</span></span>|<span data-ttu-id="9aae7-147">String</span><span class="sxs-lookup"><span data-stu-id="9aae7-147">String</span></span>|<span data-ttu-id="9aae7-148">タスク フォルダーでは、ユーザーのメールボックス内で一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="9aae7-148">The identifier of the task folder, unique in the user's mailbox.</span></span> <span data-ttu-id="9aae7-149">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9aae7-149">Read-only.</span></span>|
|<span data-ttu-id="9aae7-150">isDefaultFolder</span><span class="sxs-lookup"><span data-stu-id="9aae7-150">isDefaultFolder</span></span>|<span data-ttu-id="9aae7-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="9aae7-151">Boolean</span></span>|<span data-ttu-id="9aae7-152">フォルダーが既定のタスク フォルダーである場合は true。</span><span class="sxs-lookup"><span data-stu-id="9aae7-152">True if the folder is the default task folder.</span></span>|
|<span data-ttu-id="9aae7-153">name</span><span class="sxs-lookup"><span data-stu-id="9aae7-153">name</span></span>|<span data-ttu-id="9aae7-154">String</span><span class="sxs-lookup"><span data-stu-id="9aae7-154">String</span></span>|<span data-ttu-id="9aae7-155">タスク フォルダーの名前。</span><span class="sxs-lookup"><span data-stu-id="9aae7-155">The name of the task folder.</span></span>|
|<span data-ttu-id="9aae7-156">parentGroupKey</span><span class="sxs-lookup"><span data-stu-id="9aae7-156">parentGroupKey</span></span>|<span data-ttu-id="9aae7-157">Guid</span><span class="sxs-lookup"><span data-stu-id="9aae7-157">Guid</span></span>|<span data-ttu-id="9aae7-158">タスク フォルダーの親グループの一意の GUID 識別子。</span><span class="sxs-lookup"><span data-stu-id="9aae7-158">The unique GUID identifier for the task folder's parent group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9aae7-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9aae7-159">Relationships</span></span>
| <span data-ttu-id="9aae7-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9aae7-160">Relationship</span></span> | <span data-ttu-id="9aae7-161">型</span><span class="sxs-lookup"><span data-stu-id="9aae7-161">Type</span></span>   |<span data-ttu-id="9aae7-162">説明</span><span class="sxs-lookup"><span data-stu-id="9aae7-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9aae7-163">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="9aae7-163">multiValueExtendedProperties</span></span>|<span data-ttu-id="9aae7-164">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9aae7-164">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="9aae7-165">複数値のコレクションでは、仕事フォルダーに対して定義されたプロパティを拡張できます。</span><span class="sxs-lookup"><span data-stu-id="9aae7-165">The collection of multi-value extended properties defined for the task folder.</span></span> <span data-ttu-id="9aae7-166">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9aae7-166">Read-only.</span></span> <span data-ttu-id="9aae7-167">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="9aae7-167">Nullable.</span></span>|
|<span data-ttu-id="9aae7-168">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="9aae7-168">singleValueExtendedProperties</span></span>|<span data-ttu-id="9aae7-169">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9aae7-169">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="9aae7-170">仕事フォルダーに対して定義されている拡張プロパティを単一値のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="9aae7-170">The collection of single-value extended properties defined for the task folder.</span></span> <span data-ttu-id="9aae7-171">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9aae7-171">Read-only.</span></span> <span data-ttu-id="9aae7-172">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="9aae7-172">Nullable.</span></span>|
|<span data-ttu-id="9aae7-173">tasks</span><span class="sxs-lookup"><span data-stu-id="9aae7-173">tasks</span></span>|<span data-ttu-id="9aae7-174">[outlookTask](outlooktask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9aae7-174">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="9aae7-175">対象タスク フォルダー内のタスク。</span><span class="sxs-lookup"><span data-stu-id="9aae7-175">The tasks in this task folder.</span></span> <span data-ttu-id="9aae7-176">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9aae7-176">Read-only.</span></span> <span data-ttu-id="9aae7-177">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="9aae7-177">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9aae7-178">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9aae7-178">JSON representation</span></span>
<span data-ttu-id="9aae7-179">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9aae7-179">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "multiValueExtendedProperties",
    "singleValueExtendedProperties",
    "tasks"
  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/outlooktaskfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
