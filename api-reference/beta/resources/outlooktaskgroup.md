---
title: outlooktaskgroup リソースの種類
description: 'Outlook のタスク (outlooktask オブジェクトのコレクション) を含むフォルダーのグループ (outlooktaskfolder)。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: af5599773c6a4edef97356e99daa522760d9b37a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345535"
---
# <a name="outlooktaskgroup-resource-type"></a><span data-ttu-id="22a08-103">outlooktaskgroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="22a08-103">outlookTaskGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22a08-104">Outlook のタスク ( [outlooktask](outlooktask.md)オブジェクトのコレクション) を含むフォルダーのグループ ([outlooktaskfolder](outlooktaskfolder.md))。</span><span class="sxs-lookup"><span data-stu-id="22a08-104">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="22a08-105">Outlook には、名前を変更または削除することができない既定のタスク グループ `My Tasks` があります。</span><span class="sxs-lookup"><span data-stu-id="22a08-105">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="22a08-106">ただし、タスク グループを作成することはできます。</span><span class="sxs-lookup"><span data-stu-id="22a08-106">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="22a08-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="22a08-107">Methods</span></span>

| <span data-ttu-id="22a08-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="22a08-108">Method</span></span>           | <span data-ttu-id="22a08-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="22a08-109">Return Type</span></span>    |<span data-ttu-id="22a08-110">説明</span><span class="sxs-lookup"><span data-stu-id="22a08-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="22a08-111">outlooktaskgroup の取得</span><span class="sxs-lookup"><span data-stu-id="22a08-111">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="22a08-112">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="22a08-112">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="22a08-113">指定された Outlook タスクグループのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="22a08-113">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="22a08-114">outlooktaskfolder の作成</span><span class="sxs-lookup"><span data-stu-id="22a08-114">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="22a08-115">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="22a08-115">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="22a08-116">Outlook のタスクフォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="22a08-116">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="22a08-117">taskfolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="22a08-117">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="22a08-118">[outlooktaskfolder](outlooktaskfolder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="22a08-118">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="22a08-119">Outlook タスクフォルダーのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="22a08-119">Get a collection of Outlook task folders.</span></span>|
|[<span data-ttu-id="22a08-120">Update</span><span class="sxs-lookup"><span data-stu-id="22a08-120">Update</span></span>](../api/outlooktaskgroup-update.md) | [<span data-ttu-id="22a08-121">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="22a08-121">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="22a08-122">Outlook タスクグループの書き込み可能なプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="22a08-122">Update the writable properties of an Outlook task group.</span></span> |
|[<span data-ttu-id="22a08-123">Delete</span><span class="sxs-lookup"><span data-stu-id="22a08-123">Delete</span></span>](../api/outlooktaskgroup-delete.md) | <span data-ttu-id="22a08-124">なし</span><span class="sxs-lookup"><span data-stu-id="22a08-124">None</span></span> |<span data-ttu-id="22a08-125">指定された Outlook タスクグループを削除します。</span><span class="sxs-lookup"><span data-stu-id="22a08-125">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="22a08-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22a08-126">Properties</span></span>
| <span data-ttu-id="22a08-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22a08-127">Property</span></span>     | <span data-ttu-id="22a08-128">型</span><span class="sxs-lookup"><span data-stu-id="22a08-128">Type</span></span>   |<span data-ttu-id="22a08-129">説明</span><span class="sxs-lookup"><span data-stu-id="22a08-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22a08-130">changeKey</span><span class="sxs-lookup"><span data-stu-id="22a08-130">changeKey</span></span>|<span data-ttu-id="22a08-131">String</span><span class="sxs-lookup"><span data-stu-id="22a08-131">String</span></span>|<span data-ttu-id="22a08-132">タスク グループのバージョン。</span><span class="sxs-lookup"><span data-stu-id="22a08-132">The version of the task group.</span></span>|
|<span data-ttu-id="22a08-133">groupkey</span><span class="sxs-lookup"><span data-stu-id="22a08-133">groupKey</span></span>|<span data-ttu-id="22a08-134">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="22a08-134">Edm.Guid</span></span>|<span data-ttu-id="22a08-135">タスク グループの一意の GUID 識別子。</span><span class="sxs-lookup"><span data-stu-id="22a08-135">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="22a08-136">id</span><span class="sxs-lookup"><span data-stu-id="22a08-136">id</span></span>|<span data-ttu-id="22a08-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="22a08-137">String</span></span>|<span data-ttu-id="22a08-138">タスクグループの一意の文字列識別子。</span><span class="sxs-lookup"><span data-stu-id="22a08-138">The unique string identifier of the task group.</span></span> <span data-ttu-id="22a08-139">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="22a08-139">Read-only.</span></span>|
|<span data-ttu-id="22a08-140">isdefaultgroup</span><span class="sxs-lookup"><span data-stu-id="22a08-140">isDefaultGroup</span></span>|<span data-ttu-id="22a08-141">ブール型</span><span class="sxs-lookup"><span data-stu-id="22a08-141">Boolean</span></span>|<span data-ttu-id="22a08-142">タスク グループが既定のタスク グループの場合は true。</span><span class="sxs-lookup"><span data-stu-id="22a08-142">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="22a08-143">name</span><span class="sxs-lookup"><span data-stu-id="22a08-143">name</span></span>|<span data-ttu-id="22a08-144">String</span><span class="sxs-lookup"><span data-stu-id="22a08-144">String</span></span>|<span data-ttu-id="22a08-145">タスク グループの名前。</span><span class="sxs-lookup"><span data-stu-id="22a08-145">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22a08-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="22a08-146">Relationships</span></span>
| <span data-ttu-id="22a08-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="22a08-147">Relationship</span></span> | <span data-ttu-id="22a08-148">型</span><span class="sxs-lookup"><span data-stu-id="22a08-148">Type</span></span>   |<span data-ttu-id="22a08-149">説明</span><span class="sxs-lookup"><span data-stu-id="22a08-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22a08-150">taskfolders</span><span class="sxs-lookup"><span data-stu-id="22a08-150">taskFolders</span></span>|<span data-ttu-id="22a08-151">[outlooktaskfolder](outlooktaskfolder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="22a08-151">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="22a08-152">タスクグループ内のタスクフォルダーのコレクション。</span><span class="sxs-lookup"><span data-stu-id="22a08-152">The collection of task folders in the task group.</span></span> <span data-ttu-id="22a08-153">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="22a08-153">Read-only.</span></span> <span data-ttu-id="22a08-154">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="22a08-154">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="22a08-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="22a08-155">JSON representation</span></span>
<span data-ttu-id="22a08-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="22a08-156">Here is a JSON representation of the resource.</span></span>

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
