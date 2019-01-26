---
title: outlookTaskFolder リソースの種類
description: 'Outlook のタスク (outlookTask オブジェクトのコレクション) を含むフォルダーです。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a117e14ea1cfe4b69cbbf69720a22a0094fb0b72
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575668"
---
# <a name="outlooktaskfolder-resource-type"></a><span data-ttu-id="95e91-103">outlookTaskFolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="95e91-103">outlookTaskFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95e91-104">Outlook のタスク ( [outlookTask](outlooktask.md)オブジェクトのコレクション) を含むフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="95e91-104">A folder that contains Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="95e91-105">Outlook では、既定のタスク グループ `My Tasks` には、ユーザーのメールボックス用の既定のタスク フォルダー `Tasks` が含まれています。</span><span class="sxs-lookup"><span data-stu-id="95e91-105">In Outlook, the default task group, `My Tasks`, contains a default task folder, `Tasks`, for the user's mailbox.</span></span> <span data-ttu-id="95e91-106">これらの既定のタスク グループとフォルダーの名前を変更したり削除したりすることはできませんが、タスク グループとタスク フォルダーを作成することはできます。</span><span class="sxs-lookup"><span data-stu-id="95e91-106">You cannot rename or delete these default task group and folder, but you can create additional task groups and task folders.</span></span>


## <a name="methods"></a><span data-ttu-id="95e91-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="95e91-107">Methods</span></span>

| <span data-ttu-id="95e91-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="95e91-108">Method</span></span>           | <span data-ttu-id="95e91-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="95e91-109">Return Type</span></span>    |<span data-ttu-id="95e91-110">説明</span><span class="sxs-lookup"><span data-stu-id="95e91-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="95e91-111">OutlookTaskFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="95e91-111">Get outlookTaskFolder</span></span>](../api/outlooktaskfolder-get.md) | [<span data-ttu-id="95e91-112">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="95e91-112">outlookTaskFolder</span></span>](outlooktaskfolder.md) |<span data-ttu-id="95e91-113">プロパティと指定した Outlook の仕事フォルダーの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="95e91-113">Get the properties and relationships of the specified Outlook task folder.</span></span>|
|[<span data-ttu-id="95e91-114">OutlookTask を作成します。</span><span class="sxs-lookup"><span data-stu-id="95e91-114">Create outlookTask</span></span>](../api/outlooktaskfolder-post-tasks.md) |[<span data-ttu-id="95e91-115">outlookTask</span><span class="sxs-lookup"><span data-stu-id="95e91-115">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="95e91-116">指定されたタスクのフォルダーに Outlook のタスクを作成します。</span><span class="sxs-lookup"><span data-stu-id="95e91-116">Create an Outlook task in the specified task folder.</span></span>|
|[<span data-ttu-id="95e91-117">List tasks</span><span class="sxs-lookup"><span data-stu-id="95e91-117">List tasks</span></span>](../api/outlooktaskfolder-list-tasks.md) |<span data-ttu-id="95e91-118">[outlookTask](outlooktask.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="95e91-118">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="95e91-119">指定したフォルダーに Outlook のすべてのタスクを取得します。</span><span class="sxs-lookup"><span data-stu-id="95e91-119">Get all the Outlook tasks in the specified folder.</span></span>|
|[<span data-ttu-id="95e91-120">Update</span><span class="sxs-lookup"><span data-stu-id="95e91-120">Update</span></span>](../api/outlooktaskfolder-update.md) | [<span data-ttu-id="95e91-121">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="95e91-121">outlookTaskFolder</span></span>](outlooktaskfolder.md)   |<span data-ttu-id="95e91-122">Outlook の仕事フォルダーの書き込み可能なプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="95e91-122">Update the writable properties of an Outlook task folder.</span></span> |
|[<span data-ttu-id="95e91-123">Delete</span><span class="sxs-lookup"><span data-stu-id="95e91-123">Delete</span></span>](../api/outlooktaskfolder-delete.md) | <span data-ttu-id="95e91-124">なし</span><span class="sxs-lookup"><span data-stu-id="95e91-124">None</span></span> |<span data-ttu-id="95e91-125">指定した Outlook の仕事フォルダーを削除します。</span><span class="sxs-lookup"><span data-stu-id="95e91-125">Delete the specified Outlook task folder.</span></span>|
|<span data-ttu-id="95e91-126">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="95e91-126">**Extended properties**</span></span>| | |
|[<span data-ttu-id="95e91-127">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="95e91-127">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="95e91-128">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="95e91-128">outlookTaskFolder</span></span>](outlooktaskfolder.md)  |<span data-ttu-id="95e91-129">新規または既存の Outlook タスク フォルダー内の 1 つまたは複数の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="95e91-129">Create one or more single-value extended properties in a new or existing Outlook task folder.</span></span>   |
|[<span data-ttu-id="95e91-130">拡張プロパティを単一値を持つタスク フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="95e91-130">Get task folder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="95e91-131">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="95e91-131">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="95e91-132">拡張プロパティを使用して単一の値が含まれている Outlook の仕事フォルダーを取得する`$expand`または`$filter`。</span><span class="sxs-lookup"><span data-stu-id="95e91-132">Get Outlook task folders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="95e91-133">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="95e91-133">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="95e91-134">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="95e91-134">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="95e91-135">新規または既存の Outlook タスク フォルダー内の 1 つまたは複数の値を複数の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="95e91-135">Create one or more multi-value extended properties in a new or existing Outlook task folder.</span></span>  |
|[<span data-ttu-id="95e91-136">拡張プロパティ値を複数の作業フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="95e91-136">Get task folder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="95e91-137">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="95e91-137">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="95e91-138">使用して複数の値の拡張プロパティを含む Outlook の仕事フォルダーを取得する`$expand`。</span><span class="sxs-lookup"><span data-stu-id="95e91-138">Get an Outlook task folder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="95e91-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95e91-139">Properties</span></span>
| <span data-ttu-id="95e91-140">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95e91-140">Property</span></span>     | <span data-ttu-id="95e91-141">型</span><span class="sxs-lookup"><span data-stu-id="95e91-141">Type</span></span>   |<span data-ttu-id="95e91-142">説明</span><span class="sxs-lookup"><span data-stu-id="95e91-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95e91-143">changeKey</span><span class="sxs-lookup"><span data-stu-id="95e91-143">changeKey</span></span>|<span data-ttu-id="95e91-144">String</span><span class="sxs-lookup"><span data-stu-id="95e91-144">String</span></span>|<span data-ttu-id="95e91-145">タスク フォルダーのバージョン。</span><span class="sxs-lookup"><span data-stu-id="95e91-145">The version of the task folder.</span></span>|
|<span data-ttu-id="95e91-146">id</span><span class="sxs-lookup"><span data-stu-id="95e91-146">id</span></span>|<span data-ttu-id="95e91-147">String</span><span class="sxs-lookup"><span data-stu-id="95e91-147">String</span></span>|<span data-ttu-id="95e91-148">タスク フォルダーでは、ユーザーのメールボックス内で一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="95e91-148">The identifier of the task folder, unique in the user's mailbox.</span></span> <span data-ttu-id="95e91-149">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="95e91-149">Read-only.</span></span>|
|<span data-ttu-id="95e91-150">isDefaultFolder</span><span class="sxs-lookup"><span data-stu-id="95e91-150">isDefaultFolder</span></span>|<span data-ttu-id="95e91-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="95e91-151">Boolean</span></span>|<span data-ttu-id="95e91-152">フォルダーが既定のタスク フォルダーである場合は true。</span><span class="sxs-lookup"><span data-stu-id="95e91-152">True if the folder is the default task folder.</span></span>|
|<span data-ttu-id="95e91-153">name</span><span class="sxs-lookup"><span data-stu-id="95e91-153">name</span></span>|<span data-ttu-id="95e91-154">String</span><span class="sxs-lookup"><span data-stu-id="95e91-154">String</span></span>|<span data-ttu-id="95e91-155">タスク フォルダーの名前。</span><span class="sxs-lookup"><span data-stu-id="95e91-155">The name of the task folder.</span></span>|
|<span data-ttu-id="95e91-156">parentGroupKey</span><span class="sxs-lookup"><span data-stu-id="95e91-156">parentGroupKey</span></span>|<span data-ttu-id="95e91-157">Guid</span><span class="sxs-lookup"><span data-stu-id="95e91-157">Guid</span></span>|<span data-ttu-id="95e91-158">タスク フォルダーの親グループの一意の GUID 識別子。</span><span class="sxs-lookup"><span data-stu-id="95e91-158">The unique GUID identifier for the task folder's parent group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95e91-159">関係</span><span class="sxs-lookup"><span data-stu-id="95e91-159">Relationships</span></span>
| <span data-ttu-id="95e91-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="95e91-160">Relationship</span></span> | <span data-ttu-id="95e91-161">型</span><span class="sxs-lookup"><span data-stu-id="95e91-161">Type</span></span>   |<span data-ttu-id="95e91-162">説明</span><span class="sxs-lookup"><span data-stu-id="95e91-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95e91-163">multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="95e91-163">multiValueLegacyExtendedProperty</span></span>|<span data-ttu-id="95e91-164">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="95e91-164">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="95e91-165">複数値のコレクションでは、仕事フォルダーに対して定義されたプロパティを拡張できます。</span><span class="sxs-lookup"><span data-stu-id="95e91-165">The collection of multi-value extended properties defined for the task folder.</span></span> <span data-ttu-id="95e91-166">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="95e91-166">Read-only.</span></span> <span data-ttu-id="95e91-167">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="95e91-167">Nullable.</span></span>|
|<span data-ttu-id="95e91-168">singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="95e91-168">singleValueLegacyExtendedProperty</span></span>|<span data-ttu-id="95e91-169">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="95e91-169">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="95e91-170">仕事フォルダーに対して定義されている拡張プロパティを単一値のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="95e91-170">The collection of single-value extended properties defined for the task folder.</span></span> <span data-ttu-id="95e91-171">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="95e91-171">Read-only.</span></span> <span data-ttu-id="95e91-172">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="95e91-172">Nullable.</span></span>|
|<span data-ttu-id="95e91-173">tasks</span><span class="sxs-lookup"><span data-stu-id="95e91-173">tasks</span></span>|<span data-ttu-id="95e91-174">[outlookTask](outlooktask.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="95e91-174">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="95e91-175">対象タスク フォルダー内のタスク。</span><span class="sxs-lookup"><span data-stu-id="95e91-175">The tasks in this task folder.</span></span> <span data-ttu-id="95e91-176">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="95e91-176">Read-only.</span></span> <span data-ttu-id="95e91-177">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="95e91-177">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="95e91-178">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="95e91-178">JSON representation</span></span>
<span data-ttu-id="95e91-179">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="95e91-179">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "multiValueLegacyExtendedProperty",
    "singleValueLegacyExtendedProperty",
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
