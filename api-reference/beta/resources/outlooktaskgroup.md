---
title: outlookTaskGroup リソースの種類
description: 'Outlook のタスク (outlookTask オブジェクトのコレクション) を含むフォルダーのグループ (outlookTaskFolder)。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d519e18723ac9fbd38e7cec64a6758b0c9396bc2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966280"
---
# <a name="outlooktaskgroup-resource-type"></a><span data-ttu-id="bbdaf-103">outlookTaskGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bbdaf-103">outlookTaskGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbdaf-104">Outlook のタスク ( [Outlooktask](outlooktask.md)オブジェクトのコレクション) を含むフォルダーのグループ ([outlooktaskfolder](outlooktaskfolder.md))。</span><span class="sxs-lookup"><span data-stu-id="bbdaf-104">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="bbdaf-105">Outlook には、名前を変更または削除することができない既定のタスク グループ `My Tasks` があります。</span><span class="sxs-lookup"><span data-stu-id="bbdaf-105">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="bbdaf-106">ただし、タスク グループを作成することはできます。</span><span class="sxs-lookup"><span data-stu-id="bbdaf-106">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="bbdaf-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="bbdaf-107">Methods</span></span>

| <span data-ttu-id="bbdaf-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="bbdaf-108">Method</span></span>           | <span data-ttu-id="bbdaf-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bbdaf-109">Return Type</span></span>    |<span data-ttu-id="bbdaf-110">説明</span><span class="sxs-lookup"><span data-stu-id="bbdaf-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bbdaf-111">OutlookTaskGroup の取得</span><span class="sxs-lookup"><span data-stu-id="bbdaf-111">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="bbdaf-112">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="bbdaf-112">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="bbdaf-113">指定された Outlook タスクグループのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="bbdaf-113">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="bbdaf-114">OutlookTaskFolder の作成</span><span class="sxs-lookup"><span data-stu-id="bbdaf-114">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="bbdaf-115">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="bbdaf-115">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="bbdaf-116">Outlook のタスクフォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="bbdaf-116">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="bbdaf-117">TaskFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="bbdaf-117">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="bbdaf-118">[Outlooktaskfolder](outlooktaskfolder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bbdaf-118">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="bbdaf-119">Outlook タスクフォルダーのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="bbdaf-119">Get a collection of Outlook task folders.</span></span>|
|[<span data-ttu-id="bbdaf-120">Update</span><span class="sxs-lookup"><span data-stu-id="bbdaf-120">Update</span></span>](../api/outlooktaskgroup-update.md) | [<span data-ttu-id="bbdaf-121">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="bbdaf-121">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="bbdaf-122">Outlook タスクグループの書き込み可能なプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bbdaf-122">Update the writable properties of an Outlook task group.</span></span> |
|[<span data-ttu-id="bbdaf-123">Delete</span><span class="sxs-lookup"><span data-stu-id="bbdaf-123">Delete</span></span>](../api/outlooktaskgroup-delete.md) | <span data-ttu-id="bbdaf-124">None</span><span class="sxs-lookup"><span data-stu-id="bbdaf-124">None</span></span> |<span data-ttu-id="bbdaf-125">指定された Outlook タスクグループを削除します。</span><span class="sxs-lookup"><span data-stu-id="bbdaf-125">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="bbdaf-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bbdaf-126">Properties</span></span>
| <span data-ttu-id="bbdaf-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bbdaf-127">Property</span></span>     | <span data-ttu-id="bbdaf-128">型</span><span class="sxs-lookup"><span data-stu-id="bbdaf-128">Type</span></span>   |<span data-ttu-id="bbdaf-129">説明</span><span class="sxs-lookup"><span data-stu-id="bbdaf-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bbdaf-130">changeKey</span><span class="sxs-lookup"><span data-stu-id="bbdaf-130">changeKey</span></span>|<span data-ttu-id="bbdaf-131">String</span><span class="sxs-lookup"><span data-stu-id="bbdaf-131">String</span></span>|<span data-ttu-id="bbdaf-132">タスク グループのバージョン。</span><span class="sxs-lookup"><span data-stu-id="bbdaf-132">The version of the task group.</span></span>|
|<span data-ttu-id="bbdaf-133">groupKey</span><span class="sxs-lookup"><span data-stu-id="bbdaf-133">groupKey</span></span>|<span data-ttu-id="bbdaf-134">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="bbdaf-134">Edm.Guid</span></span>|<span data-ttu-id="bbdaf-135">タスク グループの一意の GUID 識別子。</span><span class="sxs-lookup"><span data-stu-id="bbdaf-135">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="bbdaf-136">id</span><span class="sxs-lookup"><span data-stu-id="bbdaf-136">id</span></span>|<span data-ttu-id="bbdaf-137">文字列</span><span class="sxs-lookup"><span data-stu-id="bbdaf-137">String</span></span>|<span data-ttu-id="bbdaf-138">タスクグループの一意の文字列識別子。</span><span class="sxs-lookup"><span data-stu-id="bbdaf-138">The unique string identifier of the task group.</span></span> <span data-ttu-id="bbdaf-139">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bbdaf-139">Read-only.</span></span>|
|<span data-ttu-id="bbdaf-140">isDefaultGroup</span><span class="sxs-lookup"><span data-stu-id="bbdaf-140">isDefaultGroup</span></span>|<span data-ttu-id="bbdaf-141">ブール型</span><span class="sxs-lookup"><span data-stu-id="bbdaf-141">Boolean</span></span>|<span data-ttu-id="bbdaf-142">タスク グループが既定のタスク グループの場合は true。</span><span class="sxs-lookup"><span data-stu-id="bbdaf-142">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="bbdaf-143">name</span><span class="sxs-lookup"><span data-stu-id="bbdaf-143">name</span></span>|<span data-ttu-id="bbdaf-144">String</span><span class="sxs-lookup"><span data-stu-id="bbdaf-144">String</span></span>|<span data-ttu-id="bbdaf-145">タスク グループの名前。</span><span class="sxs-lookup"><span data-stu-id="bbdaf-145">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbdaf-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bbdaf-146">Relationships</span></span>
| <span data-ttu-id="bbdaf-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bbdaf-147">Relationship</span></span> | <span data-ttu-id="bbdaf-148">型</span><span class="sxs-lookup"><span data-stu-id="bbdaf-148">Type</span></span>   |<span data-ttu-id="bbdaf-149">説明</span><span class="sxs-lookup"><span data-stu-id="bbdaf-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bbdaf-150">taskFolders</span><span class="sxs-lookup"><span data-stu-id="bbdaf-150">taskFolders</span></span>|<span data-ttu-id="bbdaf-151">[Outlooktaskfolder](outlooktaskfolder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bbdaf-151">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="bbdaf-152">タスクグループ内のタスクフォルダーのコレクション。</span><span class="sxs-lookup"><span data-stu-id="bbdaf-152">The collection of task folders in the task group.</span></span> <span data-ttu-id="bbdaf-153">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bbdaf-153">Read-only.</span></span> <span data-ttu-id="bbdaf-154">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="bbdaf-154">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bbdaf-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bbdaf-155">JSON representation</span></span>
<span data-ttu-id="bbdaf-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bbdaf-156">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
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
<!--
{
  "type": "#page.annotation",
  "description": "outlookTaskGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
