---
title: plannerTaskDetails リソースの種類
description: '**plannerTaskDetails** リソースは、タスクに関する追加情報を表します。各 task オブジェクトには詳細オブジェクトがあります。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 579ecdbf43275de90468883d158af725eb1d1734
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512312"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="a2c30-104">plannerTaskDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a2c30-104">plannerTaskDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2c30-p102">**plannerTaskDetails** リソースは、タスクに関する追加情報を表します。各 [task](plannertask.md) オブジェクトには詳細オブジェクトがあります。</span><span class="sxs-lookup"><span data-stu-id="a2c30-p102">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="a2c30-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a2c30-107">Methods</span></span>

| <span data-ttu-id="a2c30-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a2c30-108">Method</span></span>           | <span data-ttu-id="a2c30-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a2c30-109">Return Type</span></span>    |<span data-ttu-id="a2c30-110">説明</span><span class="sxs-lookup"><span data-stu-id="a2c30-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a2c30-111">Get plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="a2c30-111">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="a2c30-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="a2c30-112">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="a2c30-113">**plannerTaskDetails** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a2c30-113">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="a2c30-114">Update</span><span class="sxs-lookup"><span data-stu-id="a2c30-114">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="a2c30-115">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="a2c30-115">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="a2c30-116">**plannerTaskDetails** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="a2c30-116">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a2c30-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2c30-117">Properties</span></span>
| <span data-ttu-id="a2c30-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2c30-118">Property</span></span>     | <span data-ttu-id="a2c30-119">型</span><span class="sxs-lookup"><span data-stu-id="a2c30-119">Type</span></span>   |<span data-ttu-id="a2c30-120">説明</span><span class="sxs-lookup"><span data-stu-id="a2c30-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2c30-121">checklist</span><span class="sxs-lookup"><span data-stu-id="a2c30-121">checklist</span></span>|[<span data-ttu-id="a2c30-122">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="a2c30-122">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="a2c30-123">タスク上のチェックリスト項目のコレクション。</span><span class="sxs-lookup"><span data-stu-id="a2c30-123">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="a2c30-124">説明</span><span class="sxs-lookup"><span data-stu-id="a2c30-124">description</span></span>|<span data-ttu-id="a2c30-125">String</span><span class="sxs-lookup"><span data-stu-id="a2c30-125">String</span></span>|<span data-ttu-id="a2c30-126">タスクの説明</span><span class="sxs-lookup"><span data-stu-id="a2c30-126">Description of the task</span></span>|
|<span data-ttu-id="a2c30-127">id</span><span class="sxs-lookup"><span data-stu-id="a2c30-127">id</span></span>|<span data-ttu-id="a2c30-128">文字列</span><span class="sxs-lookup"><span data-stu-id="a2c30-128">String</span></span>| <span data-ttu-id="a2c30-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a2c30-129">Read-only.</span></span> <span data-ttu-id="a2c30-130">タスクの詳細の ID です。</span><span class="sxs-lookup"><span data-stu-id="a2c30-130">ID of the task details.</span></span> <span data-ttu-id="a2c30-131">28 の文字、大文字小文字を区別することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="a2c30-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="a2c30-132">サービスの[フォーマットの検証](tasks-identifiers-disclaimer.md)が行われます。</span><span class="sxs-lookup"><span data-stu-id="a2c30-132">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="a2c30-133">previewType</span><span class="sxs-lookup"><span data-stu-id="a2c30-133">previewType</span></span>|<span data-ttu-id="a2c30-134">string</span><span class="sxs-lookup"><span data-stu-id="a2c30-134">string</span></span>|<span data-ttu-id="a2c30-p104">タスクに表示されるプレビューの種類を設定します。使用可能な値: `automatic`、`noPreview`、`checklist`、`description`、`reference`。`automatic` に設定すると、タスクを表示しているアプリによって表示するプレビューが選択されます。</span><span class="sxs-lookup"><span data-stu-id="a2c30-p104">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="a2c30-138">references</span><span class="sxs-lookup"><span data-stu-id="a2c30-138">references</span></span>|[<span data-ttu-id="a2c30-139">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="a2c30-139">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="a2c30-140">タスク上の参照のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="a2c30-140">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2c30-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a2c30-141">Relationships</span></span>
<span data-ttu-id="a2c30-142">なし</span><span class="sxs-lookup"><span data-stu-id="a2c30-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a2c30-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a2c30-143">JSON representation</span></span>
<span data-ttu-id="a2c30-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a2c30-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannertaskdetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
