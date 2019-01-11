---
title: outlookTaskGroup リソースの種類
description: 'Outlook のタスク (outlookTask オブジェクトのコレクション) を含むフォルダー (outlookTaskFolder) のグループです。 '
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 5e885c4c8cc2abe4b3890635e010d495267dc877
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878772"
---
# <a name="outlooktaskgroup-resource-type"></a><span data-ttu-id="845cf-103">outlookTaskGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="845cf-103">outlookTaskGroup resource type</span></span>

> <span data-ttu-id="845cf-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="845cf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="845cf-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="845cf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="845cf-106">Outlook のタスク ( [outlookTask](outlooktask.md)オブジェクトのコレクション) を含むフォルダー ([outlookTaskFolder](outlooktaskfolder.md)) のグループです。</span><span class="sxs-lookup"><span data-stu-id="845cf-106">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="845cf-107">Outlook には、名前を変更または削除することができない既定のタスク グループ `My Tasks` があります。</span><span class="sxs-lookup"><span data-stu-id="845cf-107">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="845cf-108">ただし、タスク グループを作成することはできます。</span><span class="sxs-lookup"><span data-stu-id="845cf-108">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="845cf-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="845cf-109">Methods</span></span>

| <span data-ttu-id="845cf-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="845cf-110">Method</span></span>           | <span data-ttu-id="845cf-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="845cf-111">Return Type</span></span>    |<span data-ttu-id="845cf-112">説明</span><span class="sxs-lookup"><span data-stu-id="845cf-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="845cf-113">OutlookTaskGroup を取得します。</span><span class="sxs-lookup"><span data-stu-id="845cf-113">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="845cf-114">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="845cf-114">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="845cf-115">プロパティと指定した Outlook のタスク グループの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="845cf-115">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="845cf-116">OutlookTaskFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="845cf-116">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="845cf-117">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="845cf-117">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="845cf-118">Outlook の仕事フォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="845cf-118">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="845cf-119">リスト taskFolders</span><span class="sxs-lookup"><span data-stu-id="845cf-119">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="845cf-120">[outlookTaskFolder](outlooktaskfolder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="845cf-120">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="845cf-121">Outlook の仕事フォルダーのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="845cf-121">Get a collection of Outlook task folders.</span></span>|
|[<span data-ttu-id="845cf-122">Update</span><span class="sxs-lookup"><span data-stu-id="845cf-122">Update</span></span>](../api/outlooktaskgroup-update.md) | [<span data-ttu-id="845cf-123">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="845cf-123">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="845cf-124">Outlook のタスク グループの書き込み可能なプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="845cf-124">Update the writable properties of an Outlook task group.</span></span> |
|[<span data-ttu-id="845cf-125">Delete</span><span class="sxs-lookup"><span data-stu-id="845cf-125">Delete</span></span>](../api/outlooktaskgroup-delete.md) | <span data-ttu-id="845cf-126">なし</span><span class="sxs-lookup"><span data-stu-id="845cf-126">None</span></span> |<span data-ttu-id="845cf-127">指定された Outlook タスク グループを削除します。</span><span class="sxs-lookup"><span data-stu-id="845cf-127">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="845cf-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="845cf-128">Properties</span></span>
| <span data-ttu-id="845cf-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="845cf-129">Property</span></span>     | <span data-ttu-id="845cf-130">種類</span><span class="sxs-lookup"><span data-stu-id="845cf-130">Type</span></span>   |<span data-ttu-id="845cf-131">説明</span><span class="sxs-lookup"><span data-stu-id="845cf-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="845cf-132">changeKey</span><span class="sxs-lookup"><span data-stu-id="845cf-132">changeKey</span></span>|<span data-ttu-id="845cf-133">String</span><span class="sxs-lookup"><span data-stu-id="845cf-133">String</span></span>|<span data-ttu-id="845cf-134">タスク グループのバージョン。</span><span class="sxs-lookup"><span data-stu-id="845cf-134">The version of the task group.</span></span>|
|<span data-ttu-id="845cf-135">groupKey</span><span class="sxs-lookup"><span data-stu-id="845cf-135">groupKey</span></span>|<span data-ttu-id="845cf-136">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="845cf-136">Edm.Guid</span></span>|<span data-ttu-id="845cf-137">タスク グループの一意の GUID 識別子。</span><span class="sxs-lookup"><span data-stu-id="845cf-137">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="845cf-138">id</span><span class="sxs-lookup"><span data-stu-id="845cf-138">id</span></span>|<span data-ttu-id="845cf-139">String</span><span class="sxs-lookup"><span data-stu-id="845cf-139">String</span></span>|<span data-ttu-id="845cf-140">タスク グループの一意の文字列識別子です。</span><span class="sxs-lookup"><span data-stu-id="845cf-140">The unique string identifier of the task group.</span></span> <span data-ttu-id="845cf-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="845cf-141">Read-only.</span></span>|
|<span data-ttu-id="845cf-142">isDefaultGroup</span><span class="sxs-lookup"><span data-stu-id="845cf-142">isDefaultGroup</span></span>|<span data-ttu-id="845cf-143">ブール型</span><span class="sxs-lookup"><span data-stu-id="845cf-143">Boolean</span></span>|<span data-ttu-id="845cf-144">タスク グループが既定のタスク グループの場合は true。</span><span class="sxs-lookup"><span data-stu-id="845cf-144">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="845cf-145">名前</span><span class="sxs-lookup"><span data-stu-id="845cf-145">name</span></span>|<span data-ttu-id="845cf-146">String</span><span class="sxs-lookup"><span data-stu-id="845cf-146">String</span></span>|<span data-ttu-id="845cf-147">タスク グループの名前。</span><span class="sxs-lookup"><span data-stu-id="845cf-147">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="845cf-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="845cf-148">Relationships</span></span>
| <span data-ttu-id="845cf-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="845cf-149">Relationship</span></span> | <span data-ttu-id="845cf-150">型</span><span class="sxs-lookup"><span data-stu-id="845cf-150">Type</span></span>   |<span data-ttu-id="845cf-151">説明</span><span class="sxs-lookup"><span data-stu-id="845cf-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="845cf-152">taskFolders</span><span class="sxs-lookup"><span data-stu-id="845cf-152">taskFolders</span></span>|<span data-ttu-id="845cf-153">[outlookTaskFolder](outlooktaskfolder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="845cf-153">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="845cf-154">タスク グループ内のタスク フォルダーのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="845cf-154">The collection of task folders in the task group.</span></span> <span data-ttu-id="845cf-155">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="845cf-155">Read-only.</span></span> <span data-ttu-id="845cf-156">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="845cf-156">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="845cf-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="845cf-157">JSON representation</span></span>
<span data-ttu-id="845cf-158">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="845cf-158">Here is a JSON representation of the resource.</span></span>

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
