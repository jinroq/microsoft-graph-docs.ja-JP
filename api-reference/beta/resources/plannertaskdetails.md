---
title: plannerTaskDetails リソースの種類
description: '**plannerTaskDetails** リソースは、タスクに関する追加情報を表します。各 task オブジェクトには詳細オブジェクトがあります。'
localization_priority: Normal
ms.openlocfilehash: 0bec5b47d1472eae43906841c5074e4080672817
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888166"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="9c945-104">plannerTaskDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9c945-104">plannerTaskDetails resource type</span></span>

> <span data-ttu-id="9c945-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9c945-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c945-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9c945-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9c945-p103">**plannerTaskDetails** リソースは、タスクに関する追加情報を表します。各 [task](plannertask.md) オブジェクトには詳細オブジェクトがあります。</span><span class="sxs-lookup"><span data-stu-id="9c945-p103">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="9c945-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="9c945-109">Methods</span></span>

| <span data-ttu-id="9c945-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="9c945-110">Method</span></span>           | <span data-ttu-id="9c945-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9c945-111">Return Type</span></span>    |<span data-ttu-id="9c945-112">説明</span><span class="sxs-lookup"><span data-stu-id="9c945-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9c945-113">Get plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="9c945-113">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="9c945-114">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="9c945-114">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="9c945-115">**plannerTaskDetails** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="9c945-115">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="9c945-116">Update</span><span class="sxs-lookup"><span data-stu-id="9c945-116">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="9c945-117">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="9c945-117">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="9c945-118">**plannerTaskDetails** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="9c945-118">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9c945-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9c945-119">Properties</span></span>
| <span data-ttu-id="9c945-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9c945-120">Property</span></span>     | <span data-ttu-id="9c945-121">種類</span><span class="sxs-lookup"><span data-stu-id="9c945-121">Type</span></span>   |<span data-ttu-id="9c945-122">説明</span><span class="sxs-lookup"><span data-stu-id="9c945-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c945-123">checklist</span><span class="sxs-lookup"><span data-stu-id="9c945-123">checklist</span></span>|[<span data-ttu-id="9c945-124">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="9c945-124">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="9c945-125">タスク上のチェックリスト項目のコレクション。</span><span class="sxs-lookup"><span data-stu-id="9c945-125">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="9c945-126">説明</span><span class="sxs-lookup"><span data-stu-id="9c945-126">description</span></span>|<span data-ttu-id="9c945-127">String</span><span class="sxs-lookup"><span data-stu-id="9c945-127">String</span></span>|<span data-ttu-id="9c945-128">タスクの説明</span><span class="sxs-lookup"><span data-stu-id="9c945-128">Description of the task</span></span>|
|<span data-ttu-id="9c945-129">id</span><span class="sxs-lookup"><span data-stu-id="9c945-129">id</span></span>|<span data-ttu-id="9c945-130">String</span><span class="sxs-lookup"><span data-stu-id="9c945-130">String</span></span>| <span data-ttu-id="9c945-131">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9c945-131">Read-only.</span></span> <span data-ttu-id="9c945-132">タスクの詳細の ID です。</span><span class="sxs-lookup"><span data-stu-id="9c945-132">ID of the task details.</span></span> <span data-ttu-id="9c945-133">28 の文字、大文字小文字を区別することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="9c945-133">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="9c945-134">サービスの[フォーマットの検証](tasks-identifiers-disclaimer.md)が行われます。</span><span class="sxs-lookup"><span data-stu-id="9c945-134">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="9c945-135">previewType</span><span class="sxs-lookup"><span data-stu-id="9c945-135">previewType</span></span>|<span data-ttu-id="9c945-136">文字列</span><span class="sxs-lookup"><span data-stu-id="9c945-136">string</span></span>|<span data-ttu-id="9c945-p105">タスクに表示されるプレビューの種類を設定します。使用可能な値: `automatic`、`noPreview`、`checklist`、`description`、`reference`。`automatic` に設定すると、タスクを表示しているアプリによって表示するプレビューが選択されます。</span><span class="sxs-lookup"><span data-stu-id="9c945-p105">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="9c945-140">references</span><span class="sxs-lookup"><span data-stu-id="9c945-140">references</span></span>|[<span data-ttu-id="9c945-141">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="9c945-141">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="9c945-142">タスク上の参照のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="9c945-142">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c945-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9c945-143">Relationships</span></span>
<span data-ttu-id="9c945-144">なし</span><span class="sxs-lookup"><span data-stu-id="9c945-144">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9c945-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9c945-145">JSON representation</span></span>
<span data-ttu-id="9c945-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9c945-146">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
