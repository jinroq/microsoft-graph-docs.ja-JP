---
title: プラン/タスクの詳細リソースの種類
description: "\" **Plan\" Taskdetails**リソースは、タスクに関する追加情報を表します。 各 task オブジェクトには details オブジェクトがあります。"
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d22c932989b9c0d21350842babd9b4bbf420124c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035169"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="b710c-104">プラン/タスクの詳細リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b710c-104">plannerTaskDetails resource type</span></span>

<span data-ttu-id="b710c-105">" **Plan" Taskdetails**リソースは、タスクに関する追加情報を表します。</span><span class="sxs-lookup"><span data-stu-id="b710c-105">The **plannerTaskDetails** resource represents the additional information about a task.</span></span> <span data-ttu-id="b710c-106">各[task](plannertask.md)オブジェクトには details オブジェクトがあります。</span><span class="sxs-lookup"><span data-stu-id="b710c-106">Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="b710c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="b710c-107">Methods</span></span>

| <span data-ttu-id="b710c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="b710c-108">Method</span></span>           | <span data-ttu-id="b710c-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b710c-109">Return Type</span></span>    |<span data-ttu-id="b710c-110">説明</span><span class="sxs-lookup"><span data-stu-id="b710c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b710c-111">Get plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="b710c-111">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="b710c-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="b710c-112">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="b710c-113">**Plan**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b710c-113">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="b710c-114">Update</span><span class="sxs-lookup"><span data-stu-id="b710c-114">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="b710c-115">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="b710c-115">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="b710c-116">プランの更新方法の**詳細**オブジェクトを表示します。</span><span class="sxs-lookup"><span data-stu-id="b710c-116">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b710c-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b710c-117">Properties</span></span>
| <span data-ttu-id="b710c-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b710c-118">Property</span></span>     | <span data-ttu-id="b710c-119">型</span><span class="sxs-lookup"><span data-stu-id="b710c-119">Type</span></span>   |<span data-ttu-id="b710c-120">説明</span><span class="sxs-lookup"><span data-stu-id="b710c-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b710c-121">checklist</span><span class="sxs-lookup"><span data-stu-id="b710c-121">checklist</span></span>|[<span data-ttu-id="b710c-122">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="b710c-122">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="b710c-123">タスク上のチェックリスト項目のコレクション。</span><span class="sxs-lookup"><span data-stu-id="b710c-123">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="b710c-124">description</span><span class="sxs-lookup"><span data-stu-id="b710c-124">description</span></span>|<span data-ttu-id="b710c-125">String</span><span class="sxs-lookup"><span data-stu-id="b710c-125">String</span></span>|<span data-ttu-id="b710c-126">タスクの説明</span><span class="sxs-lookup"><span data-stu-id="b710c-126">Description of the task</span></span>|
|<span data-ttu-id="b710c-127">id</span><span class="sxs-lookup"><span data-stu-id="b710c-127">id</span></span>|<span data-ttu-id="b710c-128">文字列</span><span class="sxs-lookup"><span data-stu-id="b710c-128">String</span></span>| <span data-ttu-id="b710c-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b710c-129">Read-only.</span></span> <span data-ttu-id="b710c-130">タスクの詳細の ID。</span><span class="sxs-lookup"><span data-stu-id="b710c-130">ID of the task details.</span></span> <span data-ttu-id="b710c-131">28 文字長で、大文字と小文字の区別があります。</span><span class="sxs-lookup"><span data-stu-id="b710c-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="b710c-132">[書式検証](planner-identifiers-disclaimer.md)はサービスによって行われます。</span><span class="sxs-lookup"><span data-stu-id="b710c-132">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="b710c-133">previewType</span><span class="sxs-lookup"><span data-stu-id="b710c-133">previewType</span></span>|<span data-ttu-id="b710c-134">string</span><span class="sxs-lookup"><span data-stu-id="b710c-134">string</span></span>|<span data-ttu-id="b710c-135">タスクに表示されるプレビューの種類を設定します。</span><span class="sxs-lookup"><span data-stu-id="b710c-135">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="b710c-136">使用可能な値: `automatic`、`noPreview`、`checklist`、`description`、`reference`。</span><span class="sxs-lookup"><span data-stu-id="b710c-136">The possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="b710c-137">表示され`automatic`たプレビューに設定した場合は、タスクを表示するアプリによって選択されます。</span><span class="sxs-lookup"><span data-stu-id="b710c-137">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="b710c-138">references</span><span class="sxs-lookup"><span data-stu-id="b710c-138">references</span></span>|[<span data-ttu-id="b710c-139">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="b710c-139">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="b710c-140">タスク上の参照のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="b710c-140">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b710c-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b710c-141">Relationships</span></span>
<span data-ttu-id="b710c-142">なし</span><span class="sxs-lookup"><span data-stu-id="b710c-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b710c-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b710c-143">JSON representation</span></span>
<span data-ttu-id="b710c-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b710c-144">Here is a JSON representation of the resource.</span></span>

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
