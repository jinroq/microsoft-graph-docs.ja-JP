---
title: plannerTaskDetails リソースの種類
description: '**plannerTaskDetails** リソースは、タスクに関する追加情報を表します。各 task オブジェクトには詳細オブジェクトがあります。'
ms.openlocfilehash: 74ba1c5b7c607f30253463e6cfc256fd3119bf45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024012"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="582a6-104">plannerTaskDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="582a6-104">plannerTaskDetails resource type</span></span>

<span data-ttu-id="582a6-p102">**plannerTaskDetails** リソースは、タスクに関する追加情報を表します。各 [task](plannertask.md) オブジェクトには詳細オブジェクトがあります。</span><span class="sxs-lookup"><span data-stu-id="582a6-p102">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="582a6-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="582a6-107">Methods</span></span>

| <span data-ttu-id="582a6-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="582a6-108">Method</span></span>           | <span data-ttu-id="582a6-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="582a6-109">Return Type</span></span>    |<span data-ttu-id="582a6-110">説明</span><span class="sxs-lookup"><span data-stu-id="582a6-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="582a6-111">Get plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="582a6-111">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="582a6-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="582a6-112">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="582a6-113">**plannerTaskDetails** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="582a6-113">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="582a6-114">Update</span><span class="sxs-lookup"><span data-stu-id="582a6-114">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="582a6-115">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="582a6-115">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="582a6-116">**plannerTaskDetails** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="582a6-116">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="582a6-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="582a6-117">Properties</span></span>
| <span data-ttu-id="582a6-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="582a6-118">Property</span></span>     | <span data-ttu-id="582a6-119">型</span><span class="sxs-lookup"><span data-stu-id="582a6-119">Type</span></span>   |<span data-ttu-id="582a6-120">説明</span><span class="sxs-lookup"><span data-stu-id="582a6-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="582a6-121">checklist</span><span class="sxs-lookup"><span data-stu-id="582a6-121">checklist</span></span>|[<span data-ttu-id="582a6-122">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="582a6-122">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="582a6-123">タスク上のチェックリスト項目のコレクション。</span><span class="sxs-lookup"><span data-stu-id="582a6-123">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="582a6-124">説明</span><span class="sxs-lookup"><span data-stu-id="582a6-124">description</span></span>|<span data-ttu-id="582a6-125">String</span><span class="sxs-lookup"><span data-stu-id="582a6-125">String</span></span>|<span data-ttu-id="582a6-126">タスクの説明</span><span class="sxs-lookup"><span data-stu-id="582a6-126">Description of the task</span></span>|
|<span data-ttu-id="582a6-127">id</span><span class="sxs-lookup"><span data-stu-id="582a6-127">id</span></span>|<span data-ttu-id="582a6-128">String</span><span class="sxs-lookup"><span data-stu-id="582a6-128">String</span></span>| <span data-ttu-id="582a6-129">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="582a6-129">Read-only.</span></span> <span data-ttu-id="582a6-130">タスクの詳細の ID です。</span><span class="sxs-lookup"><span data-stu-id="582a6-130">ID of the task details.</span></span> <span data-ttu-id="582a6-131">28 の文字、大文字小文字を区別することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="582a6-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="582a6-132">サービスの[フォーマットの検証](planner-identifiers-disclaimer.md)が行われます。</span><span class="sxs-lookup"><span data-stu-id="582a6-132">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="582a6-133">previewType</span><span class="sxs-lookup"><span data-stu-id="582a6-133">previewType</span></span>|<span data-ttu-id="582a6-134">文字列</span><span class="sxs-lookup"><span data-stu-id="582a6-134">string</span></span>|<span data-ttu-id="582a6-135">タスクに表示されるプレビューの種類を設定します。</span><span class="sxs-lookup"><span data-stu-id="582a6-135">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="582a6-136">可能な値: `automatic`、 `noPreview`、 `checklist`、 `description`、 `reference`。</span><span class="sxs-lookup"><span data-stu-id="582a6-136">The possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="582a6-137">設定すると`automatic`、タスクを表示するアプリケーションで表示されているプレビューを選択します。</span><span class="sxs-lookup"><span data-stu-id="582a6-137">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="582a6-138">references</span><span class="sxs-lookup"><span data-stu-id="582a6-138">references</span></span>|[<span data-ttu-id="582a6-139">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="582a6-139">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="582a6-140">タスク上の参照のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="582a6-140">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="582a6-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="582a6-141">Relationships</span></span>
<span data-ttu-id="582a6-142">なし</span><span class="sxs-lookup"><span data-stu-id="582a6-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="582a6-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="582a6-143">JSON representation</span></span>
<span data-ttu-id="582a6-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="582a6-144">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
