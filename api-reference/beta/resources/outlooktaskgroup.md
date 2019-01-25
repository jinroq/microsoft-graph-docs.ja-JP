---
title: outlookTaskGroup リソースの種類
description: 'Outlook のタスク (outlookTask オブジェクトのコレクション) を含むフォルダー (outlookTaskFolder) のグループです。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 486261d80b8faad7a5969f8f1ce198479e39583c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524619"
---
# <a name="outlooktaskgroup-resource-type"></a><span data-ttu-id="c6e05-103">outlookTaskGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c6e05-103">outlookTaskGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6e05-104">Outlook のタスク ( [outlookTask](outlooktask.md)オブジェクトのコレクション) を含むフォルダー ([outlookTaskFolder](outlooktaskfolder.md)) のグループです。</span><span class="sxs-lookup"><span data-stu-id="c6e05-104">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="c6e05-105">Outlook には、名前を変更または削除することができない既定のタスク グループ `My Tasks` があります。</span><span class="sxs-lookup"><span data-stu-id="c6e05-105">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="c6e05-106">ただし、タスク グループを作成することはできます。</span><span class="sxs-lookup"><span data-stu-id="c6e05-106">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="c6e05-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c6e05-107">Methods</span></span>

| <span data-ttu-id="c6e05-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c6e05-108">Method</span></span>           | <span data-ttu-id="c6e05-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c6e05-109">Return Type</span></span>    |<span data-ttu-id="c6e05-110">説明</span><span class="sxs-lookup"><span data-stu-id="c6e05-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c6e05-111">OutlookTaskGroup を取得します。</span><span class="sxs-lookup"><span data-stu-id="c6e05-111">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="c6e05-112">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="c6e05-112">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="c6e05-113">プロパティと指定した Outlook のタスク グループの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="c6e05-113">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="c6e05-114">OutlookTaskFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="c6e05-114">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="c6e05-115">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="c6e05-115">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="c6e05-116">Outlook の仕事フォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="c6e05-116">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="c6e05-117">リスト taskFolders</span><span class="sxs-lookup"><span data-stu-id="c6e05-117">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="c6e05-118">[outlookTaskFolder](outlooktaskfolder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c6e05-118">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="c6e05-119">Outlook の仕事フォルダーのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="c6e05-119">Get a collection of Outlook task folders.</span></span>|
|[<span data-ttu-id="c6e05-120">Update</span><span class="sxs-lookup"><span data-stu-id="c6e05-120">Update</span></span>](../api/outlooktaskgroup-update.md) | [<span data-ttu-id="c6e05-121">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="c6e05-121">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="c6e05-122">Outlook のタスク グループの書き込み可能なプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c6e05-122">Update the writable properties of an Outlook task group.</span></span> |
|[<span data-ttu-id="c6e05-123">Delete</span><span class="sxs-lookup"><span data-stu-id="c6e05-123">Delete</span></span>](../api/outlooktaskgroup-delete.md) | <span data-ttu-id="c6e05-124">なし</span><span class="sxs-lookup"><span data-stu-id="c6e05-124">None</span></span> |<span data-ttu-id="c6e05-125">指定された Outlook タスク グループを削除します。</span><span class="sxs-lookup"><span data-stu-id="c6e05-125">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="c6e05-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c6e05-126">Properties</span></span>
| <span data-ttu-id="c6e05-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c6e05-127">Property</span></span>     | <span data-ttu-id="c6e05-128">型</span><span class="sxs-lookup"><span data-stu-id="c6e05-128">Type</span></span>   |<span data-ttu-id="c6e05-129">説明</span><span class="sxs-lookup"><span data-stu-id="c6e05-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6e05-130">changeKey</span><span class="sxs-lookup"><span data-stu-id="c6e05-130">changeKey</span></span>|<span data-ttu-id="c6e05-131">String</span><span class="sxs-lookup"><span data-stu-id="c6e05-131">String</span></span>|<span data-ttu-id="c6e05-132">タスク グループのバージョン。</span><span class="sxs-lookup"><span data-stu-id="c6e05-132">The version of the task group.</span></span>|
|<span data-ttu-id="c6e05-133">GroupKey</span><span class="sxs-lookup"><span data-stu-id="c6e05-133">groupKey</span></span>|<span data-ttu-id="c6e05-134">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="c6e05-134">Edm.Guid</span></span>|<span data-ttu-id="c6e05-135">タスク グループの一意の GUID 識別子。</span><span class="sxs-lookup"><span data-stu-id="c6e05-135">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="c6e05-136">id</span><span class="sxs-lookup"><span data-stu-id="c6e05-136">id</span></span>|<span data-ttu-id="c6e05-137">String</span><span class="sxs-lookup"><span data-stu-id="c6e05-137">String</span></span>|<span data-ttu-id="c6e05-138">タスク グループの一意の文字列識別子です。</span><span class="sxs-lookup"><span data-stu-id="c6e05-138">The unique string identifier of the task group.</span></span> <span data-ttu-id="c6e05-139">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c6e05-139">Read-only.</span></span>|
|<span data-ttu-id="c6e05-140">IsDefaultGroup</span><span class="sxs-lookup"><span data-stu-id="c6e05-140">isDefaultGroup</span></span>|<span data-ttu-id="c6e05-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6e05-141">Boolean</span></span>|<span data-ttu-id="c6e05-142">タスク グループが既定のタスク グループの場合は true。</span><span class="sxs-lookup"><span data-stu-id="c6e05-142">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="c6e05-143">name</span><span class="sxs-lookup"><span data-stu-id="c6e05-143">name</span></span>|<span data-ttu-id="c6e05-144">String</span><span class="sxs-lookup"><span data-stu-id="c6e05-144">String</span></span>|<span data-ttu-id="c6e05-145">タスク グループの名前。</span><span class="sxs-lookup"><span data-stu-id="c6e05-145">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6e05-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c6e05-146">Relationships</span></span>
| <span data-ttu-id="c6e05-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c6e05-147">Relationship</span></span> | <span data-ttu-id="c6e05-148">型</span><span class="sxs-lookup"><span data-stu-id="c6e05-148">Type</span></span>   |<span data-ttu-id="c6e05-149">説明</span><span class="sxs-lookup"><span data-stu-id="c6e05-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6e05-150">TaskFolders</span><span class="sxs-lookup"><span data-stu-id="c6e05-150">taskFolders</span></span>|<span data-ttu-id="c6e05-151">[outlookTaskFolder](outlooktaskfolder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c6e05-151">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="c6e05-152">タスク グループ内のタスク フォルダーのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="c6e05-152">The collection of task folders in the task group.</span></span> <span data-ttu-id="c6e05-153">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c6e05-153">Read-only.</span></span> <span data-ttu-id="c6e05-154">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="c6e05-154">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c6e05-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c6e05-155">JSON representation</span></span>
<span data-ttu-id="c6e05-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c6e05-156">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "outlookTaskGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlooktaskgroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
