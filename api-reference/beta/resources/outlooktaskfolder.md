---
title: outlookTaskFolder リソースの種類
description: 'Outlook のタスク (outlookTask オブジェクトのコレクション) を含むフォルダーです。 '
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 4b4c4bade46022b30c6e4e1f50aae58d32656f0b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882930"
---
# <a name="outlooktaskfolder-resource-type"></a><span data-ttu-id="b50b8-103">outlookTaskFolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b50b8-103">outlookTaskFolder resource type</span></span>

> <span data-ttu-id="b50b8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b50b8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b50b8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b50b8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b50b8-106">Outlook のタスク ( [outlookTask](outlooktask.md)オブジェクトのコレクション) を含むフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="b50b8-106">A folder that contains Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="b50b8-107">Outlook では、既定のタスク グループ `My Tasks` には、ユーザーのメールボックス用の既定のタスク フォルダー `Tasks` が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b50b8-107">In Outlook, the default task group, `My Tasks`, contains a default task folder, `Tasks`, for the user's mailbox.</span></span> <span data-ttu-id="b50b8-108">これらの既定のタスク グループとフォルダーの名前を変更したり削除したりすることはできませんが、タスク グループとタスク フォルダーを作成することはできます。</span><span class="sxs-lookup"><span data-stu-id="b50b8-108">You cannot rename or delete these default task group and folder, but you can create additional task groups and task folders.</span></span>


## <a name="methods"></a><span data-ttu-id="b50b8-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="b50b8-109">Methods</span></span>

| <span data-ttu-id="b50b8-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="b50b8-110">Method</span></span>           | <span data-ttu-id="b50b8-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b50b8-111">Return Type</span></span>    |<span data-ttu-id="b50b8-112">説明</span><span class="sxs-lookup"><span data-stu-id="b50b8-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b50b8-113">OutlookTaskFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="b50b8-113">Get outlookTaskFolder</span></span>](../api/outlooktaskfolder-get.md) | [<span data-ttu-id="b50b8-114">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="b50b8-114">outlookTaskFolder</span></span>](outlooktaskfolder.md) |<span data-ttu-id="b50b8-115">プロパティと指定した Outlook の仕事フォルダーの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="b50b8-115">Get the properties and relationships of the specified Outlook task folder.</span></span>|
|[<span data-ttu-id="b50b8-116">OutlookTask を作成します。</span><span class="sxs-lookup"><span data-stu-id="b50b8-116">Create outlookTask</span></span>](../api/outlooktaskfolder-post-tasks.md) |[<span data-ttu-id="b50b8-117">outlookTask</span><span class="sxs-lookup"><span data-stu-id="b50b8-117">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="b50b8-118">指定されたタスクのフォルダーに Outlook のタスクを作成します。</span><span class="sxs-lookup"><span data-stu-id="b50b8-118">Create an Outlook task in the specified task folder.</span></span>|
|[<span data-ttu-id="b50b8-119">List tasks</span><span class="sxs-lookup"><span data-stu-id="b50b8-119">List tasks</span></span>](../api/outlooktaskfolder-list-tasks.md) |<span data-ttu-id="b50b8-120">[outlookTask](outlooktask.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b50b8-120">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="b50b8-121">指定したフォルダーに Outlook のすべてのタスクを取得します。</span><span class="sxs-lookup"><span data-stu-id="b50b8-121">Get all the Outlook tasks in the specified folder.</span></span>|
|[<span data-ttu-id="b50b8-122">Update</span><span class="sxs-lookup"><span data-stu-id="b50b8-122">Update</span></span>](../api/outlooktaskfolder-update.md) | [<span data-ttu-id="b50b8-123">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="b50b8-123">outlookTaskFolder</span></span>](outlooktaskfolder.md)   |<span data-ttu-id="b50b8-124">Outlook の仕事フォルダーの書き込み可能なプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b50b8-124">Update the writable properties of an Outlook task folder.</span></span> |
|[<span data-ttu-id="b50b8-125">Delete</span><span class="sxs-lookup"><span data-stu-id="b50b8-125">Delete</span></span>](../api/outlooktaskfolder-delete.md) | <span data-ttu-id="b50b8-126">なし</span><span class="sxs-lookup"><span data-stu-id="b50b8-126">None</span></span> |<span data-ttu-id="b50b8-127">指定した Outlook の仕事フォルダーを削除します。</span><span class="sxs-lookup"><span data-stu-id="b50b8-127">Delete the specified Outlook task folder.</span></span>|
|<span data-ttu-id="b50b8-128">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="b50b8-128">**Extended properties**</span></span>| | |
|[<span data-ttu-id="b50b8-129">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="b50b8-129">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="b50b8-130">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="b50b8-130">outlookTaskFolder</span></span>](outlooktaskfolder.md)  |<span data-ttu-id="b50b8-131">新規または既存の Outlook タスク フォルダー内の 1 つまたは複数の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="b50b8-131">Create one or more single-value extended properties in a new or existing Outlook task folder.</span></span>   |
|[<span data-ttu-id="b50b8-132">拡張プロパティを単一値を持つタスク フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="b50b8-132">Get task folder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="b50b8-133">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="b50b8-133">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="b50b8-134">拡張プロパティを使用して単一の値が含まれている Outlook の仕事フォルダーを取得する`$expand`または`$filter`。</span><span class="sxs-lookup"><span data-stu-id="b50b8-134">Get Outlook task folders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="b50b8-135">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="b50b8-135">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="b50b8-136">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="b50b8-136">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="b50b8-137">新規または既存の Outlook タスク フォルダー内の 1 つまたは複数の値を複数の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="b50b8-137">Create one or more multi-value extended properties in a new or existing Outlook task folder.</span></span>  |
|[<span data-ttu-id="b50b8-138">拡張プロパティ値を複数の作業フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="b50b8-138">Get task folder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="b50b8-139">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="b50b8-139">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="b50b8-140">使用して複数の値の拡張プロパティを含む Outlook の仕事フォルダーを取得する`$expand`。</span><span class="sxs-lookup"><span data-stu-id="b50b8-140">Get an Outlook task folder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="b50b8-141">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b50b8-141">Properties</span></span>
| <span data-ttu-id="b50b8-142">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b50b8-142">Property</span></span>     | <span data-ttu-id="b50b8-143">種類</span><span class="sxs-lookup"><span data-stu-id="b50b8-143">Type</span></span>   |<span data-ttu-id="b50b8-144">説明</span><span class="sxs-lookup"><span data-stu-id="b50b8-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b50b8-145">changeKey</span><span class="sxs-lookup"><span data-stu-id="b50b8-145">changeKey</span></span>|<span data-ttu-id="b50b8-146">String</span><span class="sxs-lookup"><span data-stu-id="b50b8-146">String</span></span>|<span data-ttu-id="b50b8-147">タスク フォルダーのバージョン。</span><span class="sxs-lookup"><span data-stu-id="b50b8-147">The version of the task folder.</span></span>|
|<span data-ttu-id="b50b8-148">id</span><span class="sxs-lookup"><span data-stu-id="b50b8-148">id</span></span>|<span data-ttu-id="b50b8-149">String</span><span class="sxs-lookup"><span data-stu-id="b50b8-149">String</span></span>|<span data-ttu-id="b50b8-150">タスク フォルダーでは、ユーザーのメールボックス内で一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="b50b8-150">The identifier of the task folder, unique in the user's mailbox.</span></span> <span data-ttu-id="b50b8-151">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b50b8-151">Read-only.</span></span>|
|<span data-ttu-id="b50b8-152">isDefaultFolder</span><span class="sxs-lookup"><span data-stu-id="b50b8-152">isDefaultFolder</span></span>|<span data-ttu-id="b50b8-153">ブール型</span><span class="sxs-lookup"><span data-stu-id="b50b8-153">Boolean</span></span>|<span data-ttu-id="b50b8-154">フォルダーが既定のタスク フォルダーである場合は true。</span><span class="sxs-lookup"><span data-stu-id="b50b8-154">True if the folder is the default task folder.</span></span>|
|<span data-ttu-id="b50b8-155">名前</span><span class="sxs-lookup"><span data-stu-id="b50b8-155">name</span></span>|<span data-ttu-id="b50b8-156">String</span><span class="sxs-lookup"><span data-stu-id="b50b8-156">String</span></span>|<span data-ttu-id="b50b8-157">タスク フォルダーの名前。</span><span class="sxs-lookup"><span data-stu-id="b50b8-157">The name of the task folder.</span></span>|
|<span data-ttu-id="b50b8-158">parentGroupKey</span><span class="sxs-lookup"><span data-stu-id="b50b8-158">parentGroupKey</span></span>|<span data-ttu-id="b50b8-159">Guid</span><span class="sxs-lookup"><span data-stu-id="b50b8-159">Guid</span></span>|<span data-ttu-id="b50b8-160">タスク フォルダーの親グループの一意の GUID 識別子。</span><span class="sxs-lookup"><span data-stu-id="b50b8-160">The unique GUID identifier for the task folder's parent group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b50b8-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b50b8-161">Relationships</span></span>
| <span data-ttu-id="b50b8-162">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b50b8-162">Relationship</span></span> | <span data-ttu-id="b50b8-163">型</span><span class="sxs-lookup"><span data-stu-id="b50b8-163">Type</span></span>   |<span data-ttu-id="b50b8-164">説明</span><span class="sxs-lookup"><span data-stu-id="b50b8-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b50b8-165">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="b50b8-165">multiValueExtendedProperties</span></span>|<span data-ttu-id="b50b8-166">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="b50b8-166">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="b50b8-167">複数値のコレクションでは、仕事フォルダーに対して定義されたプロパティを拡張できます。</span><span class="sxs-lookup"><span data-stu-id="b50b8-167">The collection of multi-value extended properties defined for the task folder.</span></span> <span data-ttu-id="b50b8-168">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b50b8-168">Read-only.</span></span> <span data-ttu-id="b50b8-169">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b50b8-169">Nullable.</span></span>|
|<span data-ttu-id="b50b8-170">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="b50b8-170">singleValueExtendedProperties</span></span>|<span data-ttu-id="b50b8-171">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="b50b8-171">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="b50b8-172">仕事フォルダーに対して定義されている拡張プロパティを単一値のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="b50b8-172">The collection of single-value extended properties defined for the task folder.</span></span> <span data-ttu-id="b50b8-173">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b50b8-173">Read-only.</span></span> <span data-ttu-id="b50b8-174">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b50b8-174">Nullable.</span></span>|
|<span data-ttu-id="b50b8-175">tasks</span><span class="sxs-lookup"><span data-stu-id="b50b8-175">tasks</span></span>|<span data-ttu-id="b50b8-176">[outlookTask](outlooktask.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b50b8-176">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="b50b8-177">対象タスク フォルダー内のタスク。</span><span class="sxs-lookup"><span data-stu-id="b50b8-177">The tasks in this task folder.</span></span> <span data-ttu-id="b50b8-178">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b50b8-178">Read-only.</span></span> <span data-ttu-id="b50b8-179">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b50b8-179">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b50b8-180">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b50b8-180">JSON representation</span></span>
<span data-ttu-id="b50b8-181">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b50b8-181">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "outlookTaskFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
