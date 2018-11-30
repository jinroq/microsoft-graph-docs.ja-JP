---
title: outlookTaskGroup リソースの種類
description: 'Outlook のタスク (outlookTask オブジェクトのコレクション) を含むフォルダー (outlookTaskFolder) のグループです。 '
ms.openlocfilehash: 4896b114bf04b7e1703886453f21a4e015c9e7d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073276"
---
# <a name="outlooktaskgroup-resource-type"></a><span data-ttu-id="71ccb-103">outlookTaskGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="71ccb-103">outlookTaskGroup resource type</span></span>

> <span data-ttu-id="71ccb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="71ccb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71ccb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71ccb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="71ccb-106">Outlook のタスク ( [outlookTask](outlooktask.md)オブジェクトのコレクション) を含むフォルダー ([outlookTaskFolder](outlooktaskfolder.md)) のグループです。</span><span class="sxs-lookup"><span data-stu-id="71ccb-106">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="71ccb-107">Outlook には、名前を変更または削除することができない既定のタスク グループ `My Tasks` があります。</span><span class="sxs-lookup"><span data-stu-id="71ccb-107">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="71ccb-108">ただし、タスク グループを作成することはできます。</span><span class="sxs-lookup"><span data-stu-id="71ccb-108">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="71ccb-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="71ccb-109">Methods</span></span>

| <span data-ttu-id="71ccb-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="71ccb-110">Method</span></span>           | <span data-ttu-id="71ccb-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="71ccb-111">Return Type</span></span>    |<span data-ttu-id="71ccb-112">説明</span><span class="sxs-lookup"><span data-stu-id="71ccb-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="71ccb-113">OutlookTaskGroup を取得します。</span><span class="sxs-lookup"><span data-stu-id="71ccb-113">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="71ccb-114">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="71ccb-114">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="71ccb-115">プロパティと指定した Outlook のタスク グループの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="71ccb-115">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="71ccb-116">OutlookTaskFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="71ccb-116">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="71ccb-117">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="71ccb-117">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="71ccb-118">Outlook の仕事フォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="71ccb-118">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="71ccb-119">リスト taskFolders</span><span class="sxs-lookup"><span data-stu-id="71ccb-119">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="71ccb-120">[outlookTaskFolder](outlooktaskfolder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="71ccb-120">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="71ccb-121">Outlook の仕事フォルダーのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="71ccb-121">Get a collection of Outlook task folders.</span></span>|
|[<span data-ttu-id="71ccb-122">Update</span><span class="sxs-lookup"><span data-stu-id="71ccb-122">Update</span></span>](../api/outlooktaskgroup-update.md) | [<span data-ttu-id="71ccb-123">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="71ccb-123">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="71ccb-124">Outlook のタスク グループの書き込み可能なプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="71ccb-124">Update the writable properties of an Outlook task group.</span></span> |
|[<span data-ttu-id="71ccb-125">削除</span><span class="sxs-lookup"><span data-stu-id="71ccb-125">Delete</span></span>](../api/outlooktaskgroup-delete.md) | <span data-ttu-id="71ccb-126">なし</span><span class="sxs-lookup"><span data-stu-id="71ccb-126">None</span></span> |<span data-ttu-id="71ccb-127">指定された Outlook タスク グループを削除します。</span><span class="sxs-lookup"><span data-stu-id="71ccb-127">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="71ccb-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="71ccb-128">Properties</span></span>
| <span data-ttu-id="71ccb-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="71ccb-129">Property</span></span>     | <span data-ttu-id="71ccb-130">型</span><span class="sxs-lookup"><span data-stu-id="71ccb-130">Type</span></span>   |<span data-ttu-id="71ccb-131">説明</span><span class="sxs-lookup"><span data-stu-id="71ccb-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71ccb-132">changeKey</span><span class="sxs-lookup"><span data-stu-id="71ccb-132">changeKey</span></span>|<span data-ttu-id="71ccb-133">String</span><span class="sxs-lookup"><span data-stu-id="71ccb-133">String</span></span>|<span data-ttu-id="71ccb-134">タスク グループのバージョン。</span><span class="sxs-lookup"><span data-stu-id="71ccb-134">The version of the task group.</span></span>|
|<span data-ttu-id="71ccb-135">groupKey</span><span class="sxs-lookup"><span data-stu-id="71ccb-135">groupKey</span></span>|<span data-ttu-id="71ccb-136">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="71ccb-136">Edm.Guid</span></span>|<span data-ttu-id="71ccb-137">タスク グループの一意の GUID 識別子。</span><span class="sxs-lookup"><span data-stu-id="71ccb-137">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="71ccb-138">id</span><span class="sxs-lookup"><span data-stu-id="71ccb-138">id</span></span>|<span data-ttu-id="71ccb-139">String</span><span class="sxs-lookup"><span data-stu-id="71ccb-139">String</span></span>|<span data-ttu-id="71ccb-140">タスク グループの一意の文字列識別子です。</span><span class="sxs-lookup"><span data-stu-id="71ccb-140">The unique string identifier of the task group.</span></span> <span data-ttu-id="71ccb-141">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="71ccb-141">Read-only.</span></span>|
|<span data-ttu-id="71ccb-142">isDefaultGroup</span><span class="sxs-lookup"><span data-stu-id="71ccb-142">isDefaultGroup</span></span>|<span data-ttu-id="71ccb-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="71ccb-143">Boolean</span></span>|<span data-ttu-id="71ccb-144">タスク グループが既定のタスク グループの場合は true。</span><span class="sxs-lookup"><span data-stu-id="71ccb-144">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="71ccb-145">名前</span><span class="sxs-lookup"><span data-stu-id="71ccb-145">name</span></span>|<span data-ttu-id="71ccb-146">String</span><span class="sxs-lookup"><span data-stu-id="71ccb-146">String</span></span>|<span data-ttu-id="71ccb-147">タスク グループの名前。</span><span class="sxs-lookup"><span data-stu-id="71ccb-147">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71ccb-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="71ccb-148">Relationships</span></span>
| <span data-ttu-id="71ccb-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="71ccb-149">Relationship</span></span> | <span data-ttu-id="71ccb-150">型</span><span class="sxs-lookup"><span data-stu-id="71ccb-150">Type</span></span>   |<span data-ttu-id="71ccb-151">説明</span><span class="sxs-lookup"><span data-stu-id="71ccb-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71ccb-152">taskFolders</span><span class="sxs-lookup"><span data-stu-id="71ccb-152">taskFolders</span></span>|<span data-ttu-id="71ccb-153">[outlookTaskFolder](outlooktaskfolder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="71ccb-153">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="71ccb-154">タスク グループ内のタスク フォルダーのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="71ccb-154">The collection of task folders in the task group.</span></span> <span data-ttu-id="71ccb-155">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="71ccb-155">Read-only.</span></span> <span data-ttu-id="71ccb-156">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="71ccb-156">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="71ccb-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="71ccb-157">JSON representation</span></span>
<span data-ttu-id="71ccb-158">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="71ccb-158">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookTaskGroup"
}-->

```json
{
  "changeKey": "String",
  "groupKey": "Guid",
  "id": "String (identifier)",
  "isDefaultGroup": true,
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookTaskGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->