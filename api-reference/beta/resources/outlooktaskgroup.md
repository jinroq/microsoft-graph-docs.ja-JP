---
title: outlooktaskgroup リソースの種類
description: 'Outlook のタスク (outlooktask オブジェクトのコレクション) を含むフォルダーのグループ (outlooktaskfolder)。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 486261d80b8faad7a5969f8f1ce198479e39583c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568602"
---
# <a name="outlooktaskgroup-resource-type"></a><span data-ttu-id="9495a-103">outlooktaskgroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9495a-103">outlookTaskGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9495a-104">Outlook のタスク ( [outlooktask](outlooktask.md)オブジェクトのコレクション) を含むフォルダーのグループ ([outlooktaskfolder](outlooktaskfolder.md))。</span><span class="sxs-lookup"><span data-stu-id="9495a-104">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="9495a-105">Outlook には、名前を変更または削除することができない既定のタスク グループ `My Tasks` があります。</span><span class="sxs-lookup"><span data-stu-id="9495a-105">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="9495a-106">ただし、タスク グループを作成することはできます。</span><span class="sxs-lookup"><span data-stu-id="9495a-106">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="9495a-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="9495a-107">Methods</span></span>

| <span data-ttu-id="9495a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="9495a-108">Method</span></span>           | <span data-ttu-id="9495a-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9495a-109">Return Type</span></span>    |<span data-ttu-id="9495a-110">説明</span><span class="sxs-lookup"><span data-stu-id="9495a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9495a-111">outlooktaskgroup の取得</span><span class="sxs-lookup"><span data-stu-id="9495a-111">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="9495a-112">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="9495a-112">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="9495a-113">指定された Outlook タスクグループのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="9495a-113">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="9495a-114">outlooktaskfolder の作成</span><span class="sxs-lookup"><span data-stu-id="9495a-114">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="9495a-115">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="9495a-115">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="9495a-116">Outlook のタスクフォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="9495a-116">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="9495a-117">taskfolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="9495a-117">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="9495a-118">[outlooktaskfolder](outlooktaskfolder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9495a-118">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="9495a-119">Outlook タスクフォルダーのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="9495a-119">Get a collection of Outlook task folders.</span></span>|
|[<span data-ttu-id="9495a-120">更新する</span><span class="sxs-lookup"><span data-stu-id="9495a-120">Update</span></span>](../api/outlooktaskgroup-update.md) | [<span data-ttu-id="9495a-121">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="9495a-121">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="9495a-122">Outlook タスクグループの書き込み可能なプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9495a-122">Update the writable properties of an Outlook task group.</span></span> |
|[<span data-ttu-id="9495a-123">削除</span><span class="sxs-lookup"><span data-stu-id="9495a-123">Delete</span></span>](../api/outlooktaskgroup-delete.md) | <span data-ttu-id="9495a-124">なし</span><span class="sxs-lookup"><span data-stu-id="9495a-124">None</span></span> |<span data-ttu-id="9495a-125">指定された Outlook タスクグループを削除します。</span><span class="sxs-lookup"><span data-stu-id="9495a-125">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="9495a-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9495a-126">Properties</span></span>
| <span data-ttu-id="9495a-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9495a-127">Property</span></span>     | <span data-ttu-id="9495a-128">型</span><span class="sxs-lookup"><span data-stu-id="9495a-128">Type</span></span>   |<span data-ttu-id="9495a-129">説明</span><span class="sxs-lookup"><span data-stu-id="9495a-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9495a-130">changeKey</span><span class="sxs-lookup"><span data-stu-id="9495a-130">changeKey</span></span>|<span data-ttu-id="9495a-131">String</span><span class="sxs-lookup"><span data-stu-id="9495a-131">String</span></span>|<span data-ttu-id="9495a-132">タスク グループのバージョン。</span><span class="sxs-lookup"><span data-stu-id="9495a-132">The version of the task group.</span></span>|
|<span data-ttu-id="9495a-133">groupkey</span><span class="sxs-lookup"><span data-stu-id="9495a-133">groupKey</span></span>|<span data-ttu-id="9495a-134">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="9495a-134">Edm.Guid</span></span>|<span data-ttu-id="9495a-135">タスク グループの一意の GUID 識別子。</span><span class="sxs-lookup"><span data-stu-id="9495a-135">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="9495a-136">id</span><span class="sxs-lookup"><span data-stu-id="9495a-136">id</span></span>|<span data-ttu-id="9495a-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9495a-137">String</span></span>|<span data-ttu-id="9495a-138">タスクグループの一意の文字列識別子。</span><span class="sxs-lookup"><span data-stu-id="9495a-138">The unique string identifier of the task group.</span></span> <span data-ttu-id="9495a-139">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="9495a-139">Read-only.</span></span>|
|<span data-ttu-id="9495a-140">isdefaultgroup</span><span class="sxs-lookup"><span data-stu-id="9495a-140">isDefaultGroup</span></span>|<span data-ttu-id="9495a-141">ブール型</span><span class="sxs-lookup"><span data-stu-id="9495a-141">Boolean</span></span>|<span data-ttu-id="9495a-142">タスク グループが既定のタスク グループの場合は true。</span><span class="sxs-lookup"><span data-stu-id="9495a-142">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="9495a-143">name</span><span class="sxs-lookup"><span data-stu-id="9495a-143">name</span></span>|<span data-ttu-id="9495a-144">String</span><span class="sxs-lookup"><span data-stu-id="9495a-144">String</span></span>|<span data-ttu-id="9495a-145">タスク グループの名前。</span><span class="sxs-lookup"><span data-stu-id="9495a-145">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9495a-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9495a-146">Relationships</span></span>
| <span data-ttu-id="9495a-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9495a-147">Relationship</span></span> | <span data-ttu-id="9495a-148">型</span><span class="sxs-lookup"><span data-stu-id="9495a-148">Type</span></span>   |<span data-ttu-id="9495a-149">説明</span><span class="sxs-lookup"><span data-stu-id="9495a-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9495a-150">taskfolders</span><span class="sxs-lookup"><span data-stu-id="9495a-150">taskFolders</span></span>|<span data-ttu-id="9495a-151">[outlooktaskfolder](outlooktaskfolder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9495a-151">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="9495a-152">タスクグループ内のタスクフォルダーのコレクション。</span><span class="sxs-lookup"><span data-stu-id="9495a-152">The collection of task folders in the task group.</span></span> <span data-ttu-id="9495a-153">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="9495a-153">Read-only.</span></span> <span data-ttu-id="9495a-154">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="9495a-154">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9495a-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9495a-155">JSON representation</span></span>
<span data-ttu-id="9495a-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9495a-156">Here is a JSON representation of the resource.</span></span>

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
