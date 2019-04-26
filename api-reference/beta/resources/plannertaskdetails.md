---
title: プラン/タスクの詳細リソースの種類
description: "\" **plan\" taskdetails**リソースは、タスクに関する追加情報を表します。 各 task オブジェクトには details オブジェクトがあります。"
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: d11b0ca1f6090c65a1c5eaa45ce368d102994299
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344384"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="4fe6e-104">プラン/タスクの詳細リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4fe6e-104">plannerTaskDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fe6e-105">" **plan" taskdetails**リソースは、タスクに関する追加情報を表します。</span><span class="sxs-lookup"><span data-stu-id="4fe6e-105">The **plannerTaskDetails** resource represents the additional information about a task.</span></span> <span data-ttu-id="4fe6e-106">各[task](plannertask.md)オブジェクトには details オブジェクトがあります。</span><span class="sxs-lookup"><span data-stu-id="4fe6e-106">Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="4fe6e-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="4fe6e-107">Methods</span></span>

| <span data-ttu-id="4fe6e-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="4fe6e-108">Method</span></span>           | <span data-ttu-id="4fe6e-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4fe6e-109">Return Type</span></span>    |<span data-ttu-id="4fe6e-110">説明</span><span class="sxs-lookup"><span data-stu-id="4fe6e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4fe6e-111">Get plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="4fe6e-111">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="4fe6e-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="4fe6e-112">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="4fe6e-113">**plan**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4fe6e-113">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="4fe6e-114">更新する</span><span class="sxs-lookup"><span data-stu-id="4fe6e-114">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="4fe6e-115">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="4fe6e-115">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="4fe6e-116">プランの更新方法の**詳細**オブジェクトを表示します。</span><span class="sxs-lookup"><span data-stu-id="4fe6e-116">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4fe6e-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fe6e-117">Properties</span></span>
| <span data-ttu-id="4fe6e-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fe6e-118">Property</span></span>     | <span data-ttu-id="4fe6e-119">型</span><span class="sxs-lookup"><span data-stu-id="4fe6e-119">Type</span></span>   |<span data-ttu-id="4fe6e-120">説明</span><span class="sxs-lookup"><span data-stu-id="4fe6e-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4fe6e-121">checklist</span><span class="sxs-lookup"><span data-stu-id="4fe6e-121">checklist</span></span>|[<span data-ttu-id="4fe6e-122">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="4fe6e-122">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="4fe6e-123">タスク上のチェックリスト項目のコレクション。</span><span class="sxs-lookup"><span data-stu-id="4fe6e-123">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="4fe6e-124">description</span><span class="sxs-lookup"><span data-stu-id="4fe6e-124">description</span></span>|<span data-ttu-id="4fe6e-125">String</span><span class="sxs-lookup"><span data-stu-id="4fe6e-125">String</span></span>|<span data-ttu-id="4fe6e-126">タスクの説明</span><span class="sxs-lookup"><span data-stu-id="4fe6e-126">Description of the task</span></span>|
|<span data-ttu-id="4fe6e-127">id</span><span class="sxs-lookup"><span data-stu-id="4fe6e-127">id</span></span>|<span data-ttu-id="4fe6e-128">String</span><span class="sxs-lookup"><span data-stu-id="4fe6e-128">String</span></span>| <span data-ttu-id="4fe6e-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4fe6e-129">Read-only.</span></span> <span data-ttu-id="4fe6e-130">タスクの詳細の ID。</span><span class="sxs-lookup"><span data-stu-id="4fe6e-130">ID of the task details.</span></span> <span data-ttu-id="4fe6e-131">28 文字長で、大文字と小文字の区別があります。</span><span class="sxs-lookup"><span data-stu-id="4fe6e-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="4fe6e-132">[書式検証](tasks-identifiers-disclaimer.md)はサービスによって行われます。</span><span class="sxs-lookup"><span data-stu-id="4fe6e-132">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="4fe6e-133">previewType</span><span class="sxs-lookup"><span data-stu-id="4fe6e-133">previewType</span></span>|<span data-ttu-id="4fe6e-134">string</span><span class="sxs-lookup"><span data-stu-id="4fe6e-134">string</span></span>|<span data-ttu-id="4fe6e-p104">タスクに表示されるプレビューの種類を設定します。使用可能な値: `automatic`、`noPreview`、`checklist`、`description`、`reference`。`automatic` に設定すると、タスクを表示しているアプリによって表示するプレビューが選択されます。</span><span class="sxs-lookup"><span data-stu-id="4fe6e-p104">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="4fe6e-138">references</span><span class="sxs-lookup"><span data-stu-id="4fe6e-138">references</span></span>|[<span data-ttu-id="4fe6e-139">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="4fe6e-139">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="4fe6e-140">タスク上の参照のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="4fe6e-140">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4fe6e-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4fe6e-141">Relationships</span></span>
<span data-ttu-id="4fe6e-142">なし</span><span class="sxs-lookup"><span data-stu-id="4fe6e-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4fe6e-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4fe6e-143">JSON representation</span></span>
<span data-ttu-id="4fe6e-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4fe6e-144">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
