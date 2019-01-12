---
title: plannerExternalReference リソースの種類
description: '**PlannerExternalReference**リソース (ファイル、URL などの添付ファイル) の参照のメタデータを表します。 ExternalReferences オブジェクトのプロパティと値のペアの値です。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f95c6661dd179a7078980894b87184059598319d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952175"
---
# <a name="plannerexternalreference-resource-type"></a><span data-ttu-id="e53ab-104">plannerExternalReference リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e53ab-104">plannerExternalReference resource type</span></span>

<span data-ttu-id="e53ab-p102">**plannerExternalReference** リソースは、参照 (ファイル、URL などの添付ファイル) のメタデータを表します。[externalReferences オブジェクト](plannerexternalreferences.md)のプロパティ/値の組の値です。</span><span class="sxs-lookup"><span data-stu-id="e53ab-p102">The **plannerExternalReference** resource represents the metadata of a reference (attachments such as file, URL). It is the value of property-value pairs in the [externalReferences object](plannerexternalreferences.md).</span></span>



## <a name="properties"></a><span data-ttu-id="e53ab-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e53ab-107">Properties</span></span>
| <span data-ttu-id="e53ab-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e53ab-108">Property</span></span>     | <span data-ttu-id="e53ab-109">種類</span><span class="sxs-lookup"><span data-stu-id="e53ab-109">Type</span></span>   |<span data-ttu-id="e53ab-110">説明</span><span class="sxs-lookup"><span data-stu-id="e53ab-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e53ab-111">alias</span><span class="sxs-lookup"><span data-stu-id="e53ab-111">alias</span></span>|<span data-ttu-id="e53ab-112">String</span><span class="sxs-lookup"><span data-stu-id="e53ab-112">String</span></span>|<span data-ttu-id="e53ab-113">参照を記述するエイリアス名。</span><span class="sxs-lookup"><span data-stu-id="e53ab-113">A name alias to describe the reference.</span></span>|
|<span data-ttu-id="e53ab-114">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="e53ab-114">lastModifiedBy</span></span>|[<span data-ttu-id="e53ab-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="e53ab-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="e53ab-p103">読み取り専用です。これを最後に変更したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="e53ab-p103">Read-only. User ID by which this is last modified.</span></span>|
|<span data-ttu-id="e53ab-118">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e53ab-118">lastModifiedDateTime</span></span>|<span data-ttu-id="e53ab-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e53ab-119">DateTimeOffset</span></span>|<span data-ttu-id="e53ab-p104">読み取り専用です。これを最後に変更した日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e53ab-p104">Read-only. Date and time at which this is last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e53ab-124">previewPriority</span><span class="sxs-lookup"><span data-stu-id="e53ab-124">previewPriority</span></span>|<span data-ttu-id="e53ab-125">String</span><span class="sxs-lookup"><span data-stu-id="e53ab-125">String</span></span>|<span data-ttu-id="e53ab-126">タスクのプレビューとして参照が表示される、相対的な優先順位を設定するのに使用されます。</span><span class="sxs-lookup"><span data-stu-id="e53ab-126">Used to set the relative priority order in which the reference will be shown as a preview on the task.</span></span>|
|<span data-ttu-id="e53ab-127">type</span><span class="sxs-lookup"><span data-stu-id="e53ab-127">type</span></span>|<span data-ttu-id="e53ab-128">String</span><span class="sxs-lookup"><span data-stu-id="e53ab-128">String</span></span>|<span data-ttu-id="e53ab-p105">参照の種類を記述するのに使用されます。次の種類が含まれます: `PowerPoint`、`Word`、`Excel`、`Other`。</span><span class="sxs-lookup"><span data-stu-id="e53ab-p105">Used to describe the type of the reference. Types include: `PowerPoint`, `Word`, `Excel`, `Other`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e53ab-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e53ab-131">JSON representation</span></span>
<span data-ttu-id="e53ab-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e53ab-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerExternalReference"
}-->

```json
{
  "alias": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "previewPriority": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerExternalReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
