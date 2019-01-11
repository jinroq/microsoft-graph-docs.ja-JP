---
title: plannerTaskDetails リソースの種類
description: '**plannerTaskDetails** リソースは、タスクに関する追加情報を表します。各 task オブジェクトには詳細オブジェクトがあります。'
localization_priority: Normal
ms.openlocfilehash: a183ba0f9b19ea2de700913d29e9586442ba2c03
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806575"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="f89ec-104">plannerTaskDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f89ec-104">plannerTaskDetails resource type</span></span>

<span data-ttu-id="f89ec-p102">**plannerTaskDetails** リソースは、タスクに関する追加情報を表します。各 [task](plannertask.md) オブジェクトには詳細オブジェクトがあります。</span><span class="sxs-lookup"><span data-stu-id="f89ec-p102">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="f89ec-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="f89ec-107">Methods</span></span>

| <span data-ttu-id="f89ec-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="f89ec-108">Method</span></span>           | <span data-ttu-id="f89ec-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f89ec-109">Return Type</span></span>    |<span data-ttu-id="f89ec-110">説明</span><span class="sxs-lookup"><span data-stu-id="f89ec-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f89ec-111">Get plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="f89ec-111">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="f89ec-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="f89ec-112">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="f89ec-113">**plannerTaskDetails** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f89ec-113">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="f89ec-114">Update</span><span class="sxs-lookup"><span data-stu-id="f89ec-114">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="f89ec-115">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="f89ec-115">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="f89ec-116">**plannerTaskDetails** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="f89ec-116">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f89ec-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f89ec-117">Properties</span></span>
| <span data-ttu-id="f89ec-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f89ec-118">Property</span></span>     | <span data-ttu-id="f89ec-119">種類</span><span class="sxs-lookup"><span data-stu-id="f89ec-119">Type</span></span>   |<span data-ttu-id="f89ec-120">説明</span><span class="sxs-lookup"><span data-stu-id="f89ec-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f89ec-121">checklist</span><span class="sxs-lookup"><span data-stu-id="f89ec-121">checklist</span></span>|[<span data-ttu-id="f89ec-122">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="f89ec-122">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="f89ec-123">タスク上のチェックリスト項目のコレクション。</span><span class="sxs-lookup"><span data-stu-id="f89ec-123">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="f89ec-124">説明</span><span class="sxs-lookup"><span data-stu-id="f89ec-124">description</span></span>|<span data-ttu-id="f89ec-125">String</span><span class="sxs-lookup"><span data-stu-id="f89ec-125">String</span></span>|<span data-ttu-id="f89ec-126">タスクの説明</span><span class="sxs-lookup"><span data-stu-id="f89ec-126">Description of the task</span></span>|
|<span data-ttu-id="f89ec-127">id</span><span class="sxs-lookup"><span data-stu-id="f89ec-127">id</span></span>|<span data-ttu-id="f89ec-128">String</span><span class="sxs-lookup"><span data-stu-id="f89ec-128">String</span></span>| <span data-ttu-id="f89ec-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f89ec-129">Read-only.</span></span> <span data-ttu-id="f89ec-130">タスクの詳細の ID です。</span><span class="sxs-lookup"><span data-stu-id="f89ec-130">ID of the task details.</span></span> <span data-ttu-id="f89ec-131">28 の文字、大文字小文字を区別することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="f89ec-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="f89ec-132">サービスの[フォーマットの検証](planner-identifiers-disclaimer.md)が行われます。</span><span class="sxs-lookup"><span data-stu-id="f89ec-132">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="f89ec-133">previewType</span><span class="sxs-lookup"><span data-stu-id="f89ec-133">previewType</span></span>|<span data-ttu-id="f89ec-134">文字列</span><span class="sxs-lookup"><span data-stu-id="f89ec-134">string</span></span>|<span data-ttu-id="f89ec-135">タスクに表示されるプレビューの種類を設定します。</span><span class="sxs-lookup"><span data-stu-id="f89ec-135">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="f89ec-136">可能な値: `automatic`、 `noPreview`、 `checklist`、 `description`、 `reference`。</span><span class="sxs-lookup"><span data-stu-id="f89ec-136">The possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="f89ec-137">設定すると`automatic`、タスクを表示するアプリケーションで表示されているプレビューを選択します。</span><span class="sxs-lookup"><span data-stu-id="f89ec-137">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="f89ec-138">references</span><span class="sxs-lookup"><span data-stu-id="f89ec-138">references</span></span>|[<span data-ttu-id="f89ec-139">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="f89ec-139">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="f89ec-140">タスク上の参照のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f89ec-140">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f89ec-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f89ec-141">Relationships</span></span>
<span data-ttu-id="f89ec-142">なし</span><span class="sxs-lookup"><span data-stu-id="f89ec-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f89ec-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f89ec-143">JSON representation</span></span>
<span data-ttu-id="f89ec-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f89ec-144">Here is a JSON representation of the resource.</span></span>

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
