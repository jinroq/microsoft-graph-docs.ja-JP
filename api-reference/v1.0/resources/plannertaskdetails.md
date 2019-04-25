---
title: プラン/タスクの詳細リソースの種類
description: "\" **plan\" taskdetails**リソースは、タスクに関する追加情報を表します。 各 task オブジェクトには details オブジェクトがあります。"
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 75e17200dc52fff385c7be8fb0269a3da20464b8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534326"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="04509-104">プラン/タスクの詳細リソースの種類</span><span class="sxs-lookup"><span data-stu-id="04509-104">plannerTaskDetails resource type</span></span>

<span data-ttu-id="04509-105">" **plan" taskdetails**リソースは、タスクに関する追加情報を表します。</span><span class="sxs-lookup"><span data-stu-id="04509-105">The **plannerTaskDetails** resource represents the additional information about a task.</span></span> <span data-ttu-id="04509-106">各[task](plannertask.md)オブジェクトには details オブジェクトがあります。</span><span class="sxs-lookup"><span data-stu-id="04509-106">Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="04509-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="04509-107">Methods</span></span>

| <span data-ttu-id="04509-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="04509-108">Method</span></span>           | <span data-ttu-id="04509-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="04509-109">Return Type</span></span>    |<span data-ttu-id="04509-110">説明</span><span class="sxs-lookup"><span data-stu-id="04509-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="04509-111">Get plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="04509-111">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="04509-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="04509-112">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="04509-113">**plan**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="04509-113">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="04509-114">更新</span><span class="sxs-lookup"><span data-stu-id="04509-114">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="04509-115">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="04509-115">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="04509-116">プランの更新方法の**詳細**オブジェクトを表示します。</span><span class="sxs-lookup"><span data-stu-id="04509-116">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="04509-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04509-117">Properties</span></span>
| <span data-ttu-id="04509-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04509-118">Property</span></span>     | <span data-ttu-id="04509-119">型</span><span class="sxs-lookup"><span data-stu-id="04509-119">Type</span></span>   |<span data-ttu-id="04509-120">説明</span><span class="sxs-lookup"><span data-stu-id="04509-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04509-121">checklist</span><span class="sxs-lookup"><span data-stu-id="04509-121">checklist</span></span>|[<span data-ttu-id="04509-122">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="04509-122">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="04509-123">タスク上のチェックリスト項目のコレクション。</span><span class="sxs-lookup"><span data-stu-id="04509-123">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="04509-124">description</span><span class="sxs-lookup"><span data-stu-id="04509-124">description</span></span>|<span data-ttu-id="04509-125">String</span><span class="sxs-lookup"><span data-stu-id="04509-125">String</span></span>|<span data-ttu-id="04509-126">タスクの説明</span><span class="sxs-lookup"><span data-stu-id="04509-126">Description of the task</span></span>|
|<span data-ttu-id="04509-127">id</span><span class="sxs-lookup"><span data-stu-id="04509-127">id</span></span>|<span data-ttu-id="04509-128">String</span><span class="sxs-lookup"><span data-stu-id="04509-128">String</span></span>| <span data-ttu-id="04509-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="04509-129">Read-only.</span></span> <span data-ttu-id="04509-130">タスクの詳細の ID。</span><span class="sxs-lookup"><span data-stu-id="04509-130">ID of the task details.</span></span> <span data-ttu-id="04509-131">28 文字長で、大文字と小文字の区別があります。</span><span class="sxs-lookup"><span data-stu-id="04509-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="04509-132">[書式検証](planner-identifiers-disclaimer.md)はサービスによって行われます。</span><span class="sxs-lookup"><span data-stu-id="04509-132">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="04509-133">previewType</span><span class="sxs-lookup"><span data-stu-id="04509-133">previewType</span></span>|<span data-ttu-id="04509-134">string</span><span class="sxs-lookup"><span data-stu-id="04509-134">string</span></span>|<span data-ttu-id="04509-135">タスクに表示されるプレビューの種類を設定します。</span><span class="sxs-lookup"><span data-stu-id="04509-135">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="04509-136">使用可能な値: `automatic`、`noPreview`、`checklist`、`description`、`reference`。</span><span class="sxs-lookup"><span data-stu-id="04509-136">The possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="04509-137">表示され`automatic`たプレビューに設定した場合は、タスクを表示するアプリによって選択されます。</span><span class="sxs-lookup"><span data-stu-id="04509-137">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="04509-138">references</span><span class="sxs-lookup"><span data-stu-id="04509-138">references</span></span>|[<span data-ttu-id="04509-139">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="04509-139">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="04509-140">タスク上の参照のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="04509-140">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04509-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="04509-141">Relationships</span></span>
<span data-ttu-id="04509-142">なし</span><span class="sxs-lookup"><span data-stu-id="04509-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="04509-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="04509-143">JSON representation</span></span>
<span data-ttu-id="04509-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="04509-144">Here is a JSON representation of the resource.</span></span>

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
